# Real-world examples of Catsplit format (draft)

# structure
```
Material(
    (
        Name(),
        Tag(),
        Analysis(
            (
                Method,
                Element(
                    SiO2(Condition, Value),
                    Al2O3(Condition, Value),
                    Fe2O3(Condition, Value),
                    TiO2(Condition, Value),
                    CaO(Condition, Value),
                    Na2O(Condition, Value),
                    K2O(Condition, Value),
                    Loss(Condition, Value)
                )
            )
        ),
        Composition(
            Slipcasting(
                Stone(Condition, Value),
                Kaolin(Condition, Value),
                H2O(Condidion, Value),
                CF44(Condition, Value),
                CMC(Condition, Value),
                PVA(Condition, Value)
            ),
            Bodycasting(
                Stone(Condition, Value),
                Kaolin(Condition, Value),
                H2O(Condidion, Value),
                CMC(Condition, Value),
                PVA(Condition, Value)
            )
        ),
        Element(
            SiO2(Condition, Value),
            Al2O3(Condition, Value),
            Fe2O3(Condition, Value),
            CaO(Condition, Value),
            MgO(Condition, Value),
            Na2O(Condition, Value),
            TiO2(Condition, Value),
            MnO(Condition, Value),
            P2O5(Condition, Value),
            ZrO2(Condition, Value),
            Li2O(Condition, Value),
            SrO(Condition, Value),
            ZnO(Condition, Value),
            Cr2O3(Condition, Value),
            BaO(Condition, Value),
            Loss(Condition, Value)
        ),
        Color(
            Acid(
                Before(
                    Cie(L, a, b)
                ),
                After(
                    Cie(L, a, b)
                ),
                ~Casting
            ),
            Oxidation(
                (Temperture, Cie(L, a, b), ~Casting)
            ),
            Reduction(
                (Temperture, Cie(L, a, b), ~Casting)
            )
        ),
        Absorption(
            Oxidation(
                (Temperture, Value, ~Casting)
            ),
            Reduction(
                (Temperture, Value, ~Casting)
            )
        ),
        Shinkage(
            Oxidation(
                (Temperture, Value, ~Casting)
            ),
            Reduction(
                (Temperture, Value, ~Casting)
            )
        ),
        GrainSize(
            MeanSize(Condition, Value),
            D10(Condition, Value),
            D50(Condition, Value),
            D90(Condition, Value)
        ),
        Content(
            Quartz(Condition, Value, ~Subsequent),
            Kaolinite(Condition, Value, ~Subsequent),
            Muscovite(Condition, Value, ~Subsequent),
            Andesine(Condition, Value, ~Subsequent),
            Gibbsite(Condition, Value, ~Subsequent)
            Rutile(Condition, Value, ~Subsequent),
            Halloysite(Condition, Value, ~Subsequent),
            Rp(Condition, Value, ~Subsequent),
            Rwp(Condition, Value, ~Subsequent),
            Rexp(Condition, Value, ~Subsequent),
            X2(Condition, Value, ~Subsequent)
        )
    )
)
```
