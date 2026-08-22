# The banned number is the campaign's public contact

**Confirmed 18 Aug 2026:** Gaurang's banned number appears as the contact on **ImpactGuru**,
**Ketto**, and the **printed flyers**.

---

## First, the good news — the number is not dead

**WhatsApp banned the account, not the phone line.** The SIM still works:

| Channel | Status |
|---|---|
| Voice calls | **Working** |
| SMS | **Working** |
| WhatsApp messages | **Fail silently** — the number shows as not on WhatsApp |

So nobody has been unable to reach the family by phone. Do not panic-reprint anything.

## Now the actual damage, which is subtler and worse than a dead line

In India, a phone number on a fundraising appeal is a **WhatsApp** number by default. That is
where a donor with a question goes first — not to the dialler.

Two consequences:

1. **Silent failure.** A donor messages, sees no delivery, and gives up. Nobody learns it
   happened. There is no bounce, no missed call, no record. The campaign cannot measure what
   this is costing it.
2. **It reads as a scam signal.** This is the serious one. A medical fundraiser whose contact
   number is *not on WhatsApp* looks abandoned or fake to an Indian donor — exactly the
   suspicion a ₹26 crore ask can least afford. Someone doing basic diligence before giving
   ₹50,000 finds a number nobody is on, and quietly walks away.

The campaign's only asset is trust, and this quietly erodes it at the precise moment a
serious donor is deciding.

## Fix it today — free, no reprinting

**Replace the contact number on ImpactGuru and Ketto with Jolly's number.**

She is the Ketto campaigner, her phone is already the relay point for the family, and her
WhatsApp works. No new account, no ban-evasion question, no cost. It is a form edit on both
platforms.

- [ ] ImpactGuru — update campaigner contact number
- [ ] Ketto — update campaigner contact number
- [ ] Tell existing supporters and any WhatsApp groups: *old number is off WhatsApp, calls
      still work, use this number instead*

> ⚠ **And a warning that matters more than the fix.** If the family starts mass-forwarding
> the appeal from Jolly's number, it will be banned within weeks, exactly as Gaurang's was —
> and then the campaign has burned both numbers and looks worse each time. Her number must
> be for **receiving** contact, not broadcasting. Reach comes from supporters forwarding
> from their own accounts.

## The printed flyers

**Do not reprint yet.** The number still takes calls, so distributed flyers are degraded, not
useless — and reprinting is slow and costs money the campaign does not have.

- [ ] **Check what the QR codes actually point to.** This is the urgent part. If they encode
      a `wa.me/` link, they are **completely dead** — the scan fails, and that is far worse
      than a number that only takes calls. If they point at ImpactGuru or Ketto, they still
      work and the flyers are fine.
- [ ] For **undistributed stock**: a printed sticker over the contact line is cheap and takes
      an afternoon. Cheaper than reprinting.
- [ ] For the **next print run**: put the campaign URL on it, not a phone number.

## The structural fix, and the real argument for the domain

This is the second time in two weeks that campaign infrastructure has broken because it was
tied to something the family does not control — first the WhatsApp account, now every printed
flyer bearing its number.

**Printed material should carry `supportshaurya.in` and nothing else.** Then the contact
number, the donation links and the running total all live behind a URL the family owns, and
any of them can change without a single flyer becoming wrong.

That converts the domain from a nice-to-have into the thing that stops this happening a third
time. See [hosting.md](../platform/hosting.md).
