---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Получение аналитики
localization_priority: Normal
ms.openlocfilehash: d1f6b255747cffe7fdccb5d098e73a56151b6245
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516261"
---
# <a name="get-analytics"></a><span data-ttu-id="2db21-102">Получение аналитики</span><span class="sxs-lookup"><span data-stu-id="2db21-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2db21-103">Получите [itemAnalytics][] о представлениях, выполняемых в этом ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2db21-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="2db21-104">**ItemAnalytics** ресурсов — это удобный способ получить статистику активности для `allTime` и `lastSevenDays`.</span><span class="sxs-lookup"><span data-stu-id="2db21-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="2db21-105">Для интервала времени или интервал используйте [getActivitiesByInterval][] API.</span><span class="sxs-lookup"><span data-stu-id="2db21-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="2db21-106">**Примечание:** **ItemAnalytics** ресурсов, пока недоступна во всех [Национальный развертываний](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="2db21-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="2db21-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2db21-109">Permissions</span></span>

<span data-ttu-id="2db21-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2db21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2db21-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2db21-112">Permission type</span></span>                        | <span data-ttu-id="2db21-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2db21-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="2db21-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2db21-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2db21-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2db21-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="2db21-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2db21-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2db21-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db21-117">Not supported.</span></span>
|<span data-ttu-id="2db21-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2db21-118">Application</span></span>                            | <span data-ttu-id="2db21-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2db21-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2db21-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2db21-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="2db21-121">Пример</span><span class="sxs-lookup"><span data-stu-id="2db21-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2db21-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="2db21-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="2db21-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="2db21-123">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
