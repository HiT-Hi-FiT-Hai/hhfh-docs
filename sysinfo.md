The _HiT Hi FiT Hai_ PtokaX hub runs in a virtual environment with **QEMU** and
**KVM**. Below is the redacted output of the `dmidecode` commands both from
the physical machine as well as the virtual machine.

# Physical Machine
========================

    Handle 0x0000, DMI type 0, 24 bytes
    BIOS Information
            Vendor: American Megatrends Inc.
            Version: 0902
            Release Date: 07/05/2011
            Address: 0xF0000
            Runtime Size: 64 kB
            ROM Size: 1024 kB
            Characteristics:
                    ISA is supported
                    PCI is supported
                    PNP is supported
                    APM is supported
                    BIOS is upgradeable
                    BIOS shadowing is allowed
                    ESCD support is available
                    Boot from CD is supported
                    Selectable boot is supported
                    BIOS ROM is socketed
                    EDD is supported
                    5.25"/1.2 MB floppy services are supported (int 13h)
                    3.5"/720 kB floppy services are supported (int 13h)
                    3.5"/2.88 MB floppy services are supported (int 13h)
                    Print screen service is supported (int 5h)
                    8042 keyboard services are supported (int 9h)
                    Serial services are supported (int 14h)
                    Printer services are supported (int 17h)
                    CGA/mono video services are supported (int 10h)
                    ACPI is supported
                    USB legacy is supported
                    LS-120 boot is supported
                    ATAPI Zip drive boot is supported
                    BIOS boot specification is supported
                    Targeted content distribution is supported
            BIOS Revision: 8.14

    Handle 0x0002, DMI type 2, 15 bytes
    Base Board Information
            Manufacturer: ASUSTeK Computer INC.
            Product Name: M4N68T-M-LE-V2
            Version: Rev X.0x
            Serial Number: XXXXXXXXXXXXXXX
            Asset Tag: To Be Filled By O.E.M.
            Features:
                    Board is a hosting board
                    Board is replaceable
            Location In Chassis: To Be Filled By O.E.M.
            Chassis Handle: 0x0003
            Type: Motherboard
            Contained Object Handles: 0

    Handle 0x0004, DMI type 4, 40 bytes
    Processor Information
            Socket Designation: AM3
            Type: Central Processor
            Family: Phenom II
            Manufacturer: AMD
            ID: XX XX XX XX XX XX XX XX
            Signature: Family 16, Model 4, Stepping 3
            Flags:
                    FPU (Floating-point unit on-chip)
                    VME (Virtual mode extension)
                    DE (Debugging extension)
                    PSE (Page size extension)
                    TSC (Time stamp counter)
                    MSR (Model specific registers)
                    PAE (Physical address extension)
                    MCE (Machine check exception)
                    CX8 (CMPXCHG8 instruction supported)
                    APIC (On-chip APIC hardware supported)
                    SEP (Fast system call)
                    MTRR (Memory type range registers)
                    PGE (Page global enable)
                    MCA (Machine check architecture)
                    CMOV (Conditional move instruction supported)
                    PAT (Page attribute table)
                    PSE-36 (36-bit page size extension)
                    CLFSH (CLFLUSH instruction supported)
                    MMX (MMX technology supported)
                    FXSR (FXSAVE and FXSTOR instructions supported)
                    SSE (Streaming SIMD extensions)
                    SSE2 (Streaming SIMD extensions 2)
                    HTT (Multi-threading)
            Version: AMD Phenom(tm) II X4 965 Processor
            Voltage: 1.5 V
            External Clock: 200 MHz
            Max Speed: 3400 MHz
            Current Speed: 3400 MHz
            Status: Populated, Enabled
            Upgrade: Other
            L1 Cache Handle: 0x0005
            L2 Cache Handle: 0x0006
            L3 Cache Handle: 0x0007
            Serial Number: To Be Filled By O.E.M.
            Asset Tag: To Be Filled By O.E.M.
            Part Number: To Be Filled By O.E.M.
            Core Count: 4
            Core Enabled: 4
            Characteristics:
                    64-bit capable

    Handle 0x0005, DMI type 7, 19 bytes
    Cache Information
            Socket Designation: L1-Cache
            Configuration: Enabled, Not Socketed, Level 1
            Operational Mode: Varies With Memory Address
            Location: Internal
            Installed Size: 512 kB
            Maximum Size: 512 kB
            Supported SRAM Types:
                    Pipeline Burst
            Installed SRAM Type: Pipeline Burst
            Speed: Unknown
            Error Correction Type: Single-bit ECC
            System Type: Data
            Associativity: 4-way Set-associative

    Handle 0x0006, DMI type 7, 19 bytes
    Cache Information
            Socket Designation: L2-Cache
            Configuration: Enabled, Not Socketed, Level 2
            Operational Mode: Varies With Memory Address
            Location: Internal
            Installed Size: 2048 kB
            Maximum Size: 2048 kB
            Supported SRAM Types:
                    Pipeline Burst
            Installed SRAM Type: Pipeline Burst
            Speed: Unknown
            Error Correction Type: Single-bit ECC
            System Type: Unified
            Associativity: 4-way Set-associative

    Handle 0x0007, DMI type 7, 19 bytes
    Cache Information
            Socket Designation: L3-Cache
            Configuration: Enabled, Not Socketed, Level 3
            Operational Mode: Varies With Memory Address
            Location: Internal
            Installed Size: 6144 kB
            Maximum Size: 6144 kB
            Supported SRAM Types:
                    Pipeline Burst
            Installed SRAM Type: Pipeline Burst
            Speed: Unknown
            Error Correction Type: Single-bit ECC
            System Type: Unified
            Associativity: 4-way Set-associative

    Handle 0x0008, DMI type 5, 20 bytes
    Memory Controller Information
            Error Detecting Method: 64-bit ECC
            Error Correcting Capabilities:
                    None
            Supported Interleave: One-way Interleave
            Current Interleave: One-way Interleave
            Maximum Memory Module Size: 2048 MB
            Maximum Total Memory Size: 4096 MB
            Supported Speeds:
                    70 ns
                    60 ns
            Supported Memory Types:
                    DIMM
                    SDRAM
            Memory Module Voltage: 3.3 V
            Associated Memory Slots: 2
                    0x0009
                    0x000A
            Enabled Error Correcting Capabilities:
                    None

    Handle 0x000A, DMI type 6, 12 bytes
    Memory Module Information
            Socket Designation: DIMM1
            Bank Connections: 0 7
            Current Speed: 50 ns
            Type: ECC DIMM
            Installed Size: 4096 MB (Double-bank Connection)
            Enabled Size: 4096 MB (Double-bank Connection)
            Error Status: OK

    Handle 0x0029, DMI type 13, 22 bytes
    BIOS Language Information
            Language Description Format: Abbreviated
            Installable Languages: 1
                    en|US|iso8859-1
            Currently Installed Language: en|US|iso8859-1

    Handle 0x002A, DMI type 16, 15 bytes
    Physical Memory Array
            Location: System Board Or Motherboard
            Use: System Memory
            Error Correction Type: None
            Maximum Capacity: 8 GB
            Error Information Handle: Not Provided
            Number Of Devices: 2

    Handle 0x002B, DMI type 19, 15 bytes
    Memory Array Mapped Address
            Starting Address: 0x00000000000
            Ending Address: 0x0013FFFFFFF
            Range Size: 5 GB
            Physical Array Handle: 0x002A
            Partition Width: 1

    Handle 0x002E, DMI type 17, 27 bytes
    Memory Device
            Array Handle: 0xXXXX
            Error Information Handle: Not Provided
            Total Width: 64 bits
            Data Width: 64 bits
            Size: 4096 MB
            Form Factor: DIMM
            Set: None
            Locator: DIMM1
            Bank Locator: BANK1
            Type: Other
            Type Detail: Synchronous
            Speed: 1333 MHz
            Manufacturer: Manufacturer1
            Serial Number: SerNum1
            Asset Tag: AssetTagNum1
            Part Number: PartNum1

# Virtual Machine
========================

    Handle 0x0000, DMI type 0, 24 bytes
    BIOS Information
            Vendor: Bochs
            Version: Bochs
            Release Date: 01/01/2007
            Address: 0xE8000
            Runtime Size: 96 kB
            ROM Size: 64 kB
            Characteristics:
                    BIOS characteristics not supported
                    Targeted content distribution is supported
            BIOS Revision: 1.0

    Handle 0x0100, DMI type 1, 27 bytes
    System Information
            Manufacturer: Bochs
            Product Name: Bochs
            Version: Not Specified
            Serial Number: Not Specified
            UUID: 066531BB-6EDD-F3EC-66BA-250CF13A41D8
            Wake-up Type: Power Switch
            SKU Number: Not Specified
            Family: Not Specified

    Handle 0x0300, DMI type 3, 20 bytes
    Chassis Information
            Manufacturer: Bochs
            Type: Other
            Lock: Not Present
            Version: Not Specified
            Serial Number: Not Specified
            Asset Tag: Not Specified
            Boot-up State: Safe
            Power Supply State: Safe
            Thermal State: Safe
            Security Status: Unknown
            OEM Information: 0x00000000
            Height: Unspecified
            Number Of Power Cords: Unspecified

    Handle 0x0401, DMI type 4, 32 bytes
    Processor Information
            Socket Designation: CPU 1
            Type: Central Processor
            Family: Other
            Manufacturer: Bochs
            ID: 61 0F 00 00 FF FB 8B 07
            Version: Not Specified
            Voltage: Unknown
            External Clock: Unknown
            Max Speed: 2000 MHz
            Current Speed: 2000 MHz
            Status: Populated, Enabled
            Upgrade: Other
            L1 Cache Handle: Not Provided
            L2 Cache Handle: Not Provided
            L3 Cache Handle: Not Provided

    Handle 0x1000, DMI type 16, 15 bytes
    Physical Memory Array
            Location: Other
            Use: System Memory
            Error Correction Type: Multi-bit ECC
            Maximum Capacity: 1 GB
            Error Information Handle: Not Provided
            Number Of Devices: 1

    Handle 0x1100, DMI type 17, 21 bytes
    Memory Device
            Array Handle: 0x1000
            Error Information Handle: 0x0305
            Total Width: 64 bits
            Data Width: 64 bits
            Size: 1024 MB
            Form Factor: DIMM
            Set: None
            Locator: DIMM 0
            Bank Locator: Not Specified
            Type: RAM
            Type Detail: None

    Handle 0x1300, DMI type 19, 15 bytes
    Memory Array Mapped Address
            Starting Address: 0x00000000000
            Ending Address: 0x0003FFFFFFF
            Range Size: 1 GB
            Physical Array Handle: 0x1000
            Partition Width: 1

    Handle 0x1400, DMI type 20, 19 bytes
    Memory Device Mapped Address
            Starting Address: 0x00000000000
            Ending Address: 0x0003FFFFFFF
            Range Size: 1 GB
            Physical Device Handle: 0x1100
            Memory Array Mapped Address Handle: 0x1300
            Partition Row Position: 1
