# RC13 commerce hardening

Sandbox only. Added expiring inventory reservations (default 15 minutes), automatic release on subsequent API requests, delivery address collection, constrained admin state transitions, supplier-acceptance gate before fulfilment, and real delivery details in supplier submission.

NOT COMPLETE: Real supplier contract, verified stock/prices, live PayFast merchant, public HTTPS deployment, durable production database, webhook reverse-proxy/IP configuration, shipping rates, refund workflow, and real end-to-end tests. Do not enable production payments.

To run locally: `cd commerce && python -m unittest discover -v && python sandbox_server.py`. The checkout HTML requires a deployed HTTPS API URL. Supplier API remains disabled until verified.
