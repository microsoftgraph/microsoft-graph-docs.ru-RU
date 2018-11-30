---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Получение аналитики
ms.openlocfilehash: 57f009e0d2a07a5bf8c9a0f3b3617083bc279545
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079067"
---
# <a name="get-analytics"></a><span data-ttu-id="d85e7-102">Получение аналитики</span><span class="sxs-lookup"><span data-stu-id="d85e7-102">Get analytics</span></span>

> <span data-ttu-id="d85e7-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d85e7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d85e7-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d85e7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d85e7-105">Получите [itemAnalytics][] о представлениях, выполняемых в этом ресурсе.</span><span class="sxs-lookup"><span data-stu-id="d85e7-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="d85e7-106">**ItemAnalytics** ресурсов — это удобный способ получить статистику активности для `allTime` и `lastSevenDays`.</span><span class="sxs-lookup"><span data-stu-id="d85e7-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="d85e7-107">Для интервала времени или интервал используйте [getActivitiesByInterval][] API.</span><span class="sxs-lookup"><span data-stu-id="d85e7-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="d85e7-108">**Примечание:** **ItemAnalytics** ресурсов, пока недоступна во всех [Национальный развертываний](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="d85e7-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="d85e7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d85e7-111">Permissions</span></span>

<span data-ttu-id="d85e7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d85e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d85e7-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d85e7-114">Permission type</span></span>                        | <span data-ttu-id="d85e7-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d85e7-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d85e7-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d85e7-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d85e7-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d85e7-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d85e7-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d85e7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d85e7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d85e7-119">Not supported.</span></span>
|<span data-ttu-id="d85e7-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d85e7-120">Application</span></span>                            | <span data-ttu-id="d85e7-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d85e7-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d85e7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d85e7-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="d85e7-123">Пример</span><span class="sxs-lookup"><span data-stu-id="d85e7-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d85e7-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="d85e7-124">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="d85e7-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="d85e7-125">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics"
} -->
