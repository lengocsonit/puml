# puml
@startuml

class SystemMemory {
    - {static} int WORD_LENGTH = 16
    - {static} int BYTE_LENGTH = 8
    # uint address
    # uint size
    # ulong[] rawData
    + enum UnitFunctionSupportStatus
    + enum SupportStatus
    + enum OperationState
    + enum SlaveInstalledCountValue
    + {static} GetBitValue(ulong value, int bitIndex): int
    + {static} WordToDWord(ulong wordHigh, wordLow): ulong
    + WordToDWord(int high, int low): ulong
    + SystemMemory(uint adress, uint size)
    + {virtual} Update(): bool



}

@enduml
