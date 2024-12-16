# WorkerProtocol in SlinkyL1

The **WorkerProtocol** is an assigned role in the slinky network to complete certain tasks assigned to the worker. These tasks include various functions that are under development. There are hopes of extendability using a repository system.

## The Worker Protocol In Rust

```rust
use serde::{Serialize,Deserialize};

/// # WorkerProtocolRequest
///
/// Request a response for WorkerProtocol
pub struct WorkerProtocolRequest {
    // Request Task Output
    req_task: WorkerTaskID,

    // Flags
    action: u16,
    input: String,
}

pub struct SlinkWorker<T> {
    tasks: Vec<
    schema: T
}


pub struct WorkerSchema {
    // Internet Address Controlled By SlinkDNS and Pivot
    // Uses Intense PoW to retrieve or allows buying depending on Pivot
    ia: InternetAddress,

    pk: PublicKey,
    pq_pk: PqPublicKey,

    signature: Signature,
    
    
}

// Primitives

pub struct WorkerTaskLocation(&str);
pub struct WorkerTaskName(&str);
pub struct WorkerTaskID(u16);

```

These workers can act as **Services** for others.

## Type of Tasks

1. General Tasks (Built-In)
2. Custom Tasks By SlinkyRepo
