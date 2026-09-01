# Resident Evil 2 Leon feasibility

## Current result

The `main` branch binds the owned USA Dual Shock Leon program `SLUS_007.48`
to PSXRecomp `8b4e0900`. The probe found a 987,136-byte program with entry
point `0x80078408` and SHA-256
`E576348F64D015ECFF6E1CE875A8924EE252BA7F3F9478B0917CBBDEB97DB441`.

The Claire disc uses a different program. It is qualified independently on
branch `program/claire`. The stable framework does not combine these programs
into one setup host. This source tree contains no retail input or private path.

## Known boundary

Each program needs its own clean build, package, startup, save, scenario, media,
audio, controller, and gameplay evidence. A Leon pass does not qualify Claire,
and a Claire pass does not qualify Leon. Their package prefixes stay distinct.

Experimental decompilation and function overrides remain outside this source.
They can enter stable source only after equivalence, deterministic fallback,
and removal or acceptance gates pass.

## Next gate

Build and package the Leon branch from a clean checkout. Generate from the
owned Leon disc in an ignored directory and run a hidden startup test. Alex
must complete the visible manual route before any release.
