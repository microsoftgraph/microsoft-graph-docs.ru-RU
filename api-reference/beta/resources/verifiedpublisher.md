---
title: Тип ресурса Верифиедпублишер
description: Представляет проверенного издателя приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: 0d704b42c83a853d094406c0ba62010da30ce142
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471577"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="53f2d-103">Тип ресурса Верифиедпублишер</span><span class="sxs-lookup"><span data-stu-id="53f2d-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="53f2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53f2d-105">Представляет проверенного издателя [приложения](application.md).</span><span class="sxs-lookup"><span data-stu-id="53f2d-105">Represents a verified publisher of an [application](application.md).</span></span> <span data-ttu-id="53f2d-106">Для получения дополнительных сведений см [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="53f2d-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="53f2d-107">Проверенные издатели задаются с помощью [сетверифиедпублишер](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [унсетверифиедпублишер](../api/application-unsetverifiedpublisher.md).</span><span class="sxs-lookup"><span data-stu-id="53f2d-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="53f2d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="53f2d-108">Properties</span></span>

| <span data-ttu-id="53f2d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="53f2d-109">Property</span></span> | <span data-ttu-id="53f2d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="53f2d-110">Type</span></span> | <span data-ttu-id="53f2d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="53f2d-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="53f2d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="53f2d-112">displayName</span></span>|<span data-ttu-id="53f2d-113">String</span><span class="sxs-lookup"><span data-stu-id="53f2d-113">String</span></span>|<span data-ttu-id="53f2d-114">Проверенное имя издателя из учетной записи Microsoft партнерской сети организации (МПН) издателя приложения.</span><span class="sxs-lookup"><span data-stu-id="53f2d-114">The verified publisher name from the app publisher's Microsoft Partner Network (MPN) account.</span></span>|
|<span data-ttu-id="53f2d-115">верифиедпублишерид</span><span class="sxs-lookup"><span data-stu-id="53f2d-115">verifiedPublisherId</span></span>|<span data-ttu-id="53f2d-116">String</span><span class="sxs-lookup"><span data-stu-id="53f2d-116">String</span></span>| <span data-ttu-id="53f2d-117">Идентификатор проверенного издателя из учетной записи центра партнера издателя приложения.</span><span class="sxs-lookup"><span data-stu-id="53f2d-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="53f2d-118">аддеддатетиме</span><span class="sxs-lookup"><span data-stu-id="53f2d-118">addedDateTime</span></span>|<span data-ttu-id="53f2d-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="53f2d-119">DateTimeOffSet</span></span>| <span data-ttu-id="53f2d-120">Временная метка при первом добавлении проверенного издателя или последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="53f2d-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="53f2d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53f2d-121">JSON representation</span></span>
<span data-ttu-id="53f2d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53f2d-122">Here is a JSON representation of the resource.</span></span>

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
