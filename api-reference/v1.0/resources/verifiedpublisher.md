---
title: Тип ресурса verifiedPublisher
description: Представляет проверенного издателя приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 0c7d500a4fd032704f36953c8bf18efe6fa0f68d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129681"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="ade22-103">Тип ресурса verifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="ade22-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="ade22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ade22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ade22-105">Представляет проверенного издателя [приложения.](application.md)</span><span class="sxs-lookup"><span data-stu-id="ade22-105">Represents the verified publisher of the [application](application.md).</span></span> <span data-ttu-id="ade22-106">Дополнительные сведения см. в [проверке Publisher.](/azure/active-directory/develop/publisher-verification-overview)</span><span class="sxs-lookup"><span data-stu-id="ade22-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="ade22-107">Проверенные издатели устанавливаются с помощью [setVerifiedPublisher](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [unsetVerifiedPublisher.](../api/application-unsetverifiedpublisher.md)</span><span class="sxs-lookup"><span data-stu-id="ade22-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ade22-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ade22-108">Properties</span></span>

| <span data-ttu-id="ade22-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ade22-109">Property</span></span> | <span data-ttu-id="ade22-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ade22-110">Type</span></span> | <span data-ttu-id="ade22-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ade22-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ade22-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ade22-112">displayName</span></span>|<span data-ttu-id="ade22-113">String</span><span class="sxs-lookup"><span data-stu-id="ade22-113">String</span></span>|<span data-ttu-id="ade22-114">Проверенное имя издателя из учетной записи Центра партнеров издателя приложения.</span><span class="sxs-lookup"><span data-stu-id="ade22-114">The verified publisher name from the app publisher's Partner Center account.</span></span>|
|<span data-ttu-id="ade22-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="ade22-115">verifiedPublisherId</span></span>|<span data-ttu-id="ade22-116">String</span><span class="sxs-lookup"><span data-stu-id="ade22-116">String</span></span>| <span data-ttu-id="ade22-117">ИД проверенного издателя из учетной записи Центра партнеров издателя приложений.</span><span class="sxs-lookup"><span data-stu-id="ade22-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="ade22-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="ade22-118">addedDateTime</span></span>|<span data-ttu-id="ade22-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="ade22-119">DateTimeOffSet</span></span>| <span data-ttu-id="ade22-120">Временнаямпетка первого или последнего обновления проверенного издателя.</span><span class="sxs-lookup"><span data-stu-id="ade22-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="ade22-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ade22-121">JSON representation</span></span>
<span data-ttu-id="ade22-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ade22-122">Here is a JSON representation of the resource.</span></span>

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


<!-- uuid: 7a355221-34dd-4579-9bdd-4c3e1909e1bb
2020-09-09 20:45:56 UTC -->
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
