---
title: Тип ресурса verifiedPublisher
description: Представляет проверенного издателя приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 5acc66bd72c65b25d8301c4870fa5ff0f98a0d73
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135627"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="c1617-103">Тип ресурса verifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="c1617-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="c1617-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1617-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1617-105">Представляет проверенного издателя [приложения.](application.md)</span><span class="sxs-lookup"><span data-stu-id="c1617-105">Represents a verified publisher of an [application](application.md).</span></span> <span data-ttu-id="c1617-106">Дополнительные сведения см. в [проверке Publisher.](/azure/active-directory/develop/publisher-verification-overview)</span><span class="sxs-lookup"><span data-stu-id="c1617-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="c1617-107">Проверенные издатели устанавливаются с помощью [setVerifiedPublisher](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [unsetVerifiedPublisher.](../api/application-unsetverifiedpublisher.md)</span><span class="sxs-lookup"><span data-stu-id="c1617-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1617-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1617-108">Properties</span></span>

| <span data-ttu-id="c1617-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1617-109">Property</span></span> | <span data-ttu-id="c1617-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c1617-110">Type</span></span> | <span data-ttu-id="c1617-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1617-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c1617-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c1617-112">displayName</span></span>|<span data-ttu-id="c1617-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c1617-113">String</span></span>|<span data-ttu-id="c1617-114">Проверенное имя издателя из учетной записи Microsoft Partner Network (MPN) издателя приложения.</span><span class="sxs-lookup"><span data-stu-id="c1617-114">The verified publisher name from the app publisher's Microsoft Partner Network (MPN) account.</span></span>|
|<span data-ttu-id="c1617-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="c1617-115">verifiedPublisherId</span></span>|<span data-ttu-id="c1617-116">Строка</span><span class="sxs-lookup"><span data-stu-id="c1617-116">String</span></span>| <span data-ttu-id="c1617-117">ИД проверенного издателя из учетной записи Центра партнеров издателя приложений.</span><span class="sxs-lookup"><span data-stu-id="c1617-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="c1617-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1617-118">addedDateTime</span></span>|<span data-ttu-id="c1617-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="c1617-119">DateTimeOffSet</span></span>| <span data-ttu-id="c1617-120">Временнаямпетка первого или последнего обновления проверенного издателя.</span><span class="sxs-lookup"><span data-stu-id="c1617-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c1617-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c1617-121">JSON representation</span></span>
<span data-ttu-id="c1617-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1617-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedPublisher"
}-->

```json
{
  "displayName": "String",
  "verifiedPublisherId": "String",
  "addedDateTime": "DateTimeOffSet"
}

```


<!-- uuid: e9aa37e1-f0b7-4201-a6b2-d26ce091dff6
2020-09-09 20:42:32 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedPublisher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
