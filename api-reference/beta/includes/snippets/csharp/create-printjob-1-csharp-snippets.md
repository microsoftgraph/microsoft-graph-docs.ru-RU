---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 787fa46522f2f0897e9472eb17a05e44b3dc946ff4fe3ede034c3f2baf40b505
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138094"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = new PrintJob
{
    Configuration = new PrintJobConfiguration
    {
        FeedOrientation = PrinterFeedOrientation.LongEdgeFirst,
        PageRanges = new List<IntegerRange>()
        {
            new IntegerRange
            {
                Start = 1,
                End = 1
            }
        },
        Quality = PrintQuality.Medium,
        Dpi = 600,
        Orientation = PrintOrientation.Landscape,
        Copies = 1,
        DuplexMode = PrintDuplexMode.OneSided,
        ColorMode = PrintColorMode.BlackAndWhite,
        InputBin = "by-pass-tray",
        OutputBin = "output-tray",
        MediaSize = "A4",
        Margin = new PrintMargin
        {
            Top = 0,
            Bottom = 0,
            Left = 0,
            Right = 0
        },
        MediaType = "stationery",
        Finishings = null,
        PagesPerSheet = 1,
        MultipageLayout = PrintMultipageLayout.ClockwiseFromBottomLeft,
        Collate = false,
        Scaling = PrintScaling.ShrinkToFit,
        FitPdfToPage = false
    }
};

await graphClient.Print.Printers["{printer-id}"].Jobs
    .Request()
    .AddAsync(printJob);

```