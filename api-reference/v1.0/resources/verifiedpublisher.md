---
title: Тип ресурса Верифиедпублишер
description: Представляет проверенного издателя приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: d998b8bf3e5ab4ad253e31a96794e8e531e6803e
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921901"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="9a9aa-103">Тип ресурса Верифиедпублишер</span><span class="sxs-lookup"><span data-stu-id="9a9aa-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="9a9aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a9aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a9aa-105">Представляет проверенного издателя [приложения](application.md).</span><span class="sxs-lookup"><span data-stu-id="9a9aa-105">Represents the verified publisher of the [application](application.md).</span></span> <span data-ttu-id="9a9aa-106">Для получения дополнительных сведений см [Проверка издателя](/azure/active-directory/develop/publisher-verification-overview).</span><span class="sxs-lookup"><span data-stu-id="9a9aa-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="9a9aa-107">Проверенные издатели задаются с помощью [сетверифиедпублишер](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [унсетверифиедпублишер](../api/application-unsetverifiedpublisher.md).</span><span class="sxs-lookup"><span data-stu-id="9a9aa-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9a9aa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a9aa-108">Properties</span></span>

| <span data-ttu-id="9a9aa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a9aa-109">Property</span></span> | <span data-ttu-id="9a9aa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9a9aa-110">Type</span></span> | <span data-ttu-id="9a9aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9a9aa-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9a9aa-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9a9aa-112">displayName</span></span>|<span data-ttu-id="9a9aa-113">String</span><span class="sxs-lookup"><span data-stu-id="9a9aa-113">String</span></span>|<span data-ttu-id="9a9aa-114">Проверенное имя издателя из учетной записи центра партнера издателя приложения.</span><span class="sxs-lookup"><span data-stu-id="9a9aa-114">The verified publisher name from the app publisher's Partner Center account.</span></span>|
|<span data-ttu-id="9a9aa-115">верифиедпублишерид</span><span class="sxs-lookup"><span data-stu-id="9a9aa-115">verifiedPublisherId</span></span>|<span data-ttu-id="9a9aa-116">String</span><span class="sxs-lookup"><span data-stu-id="9a9aa-116">String</span></span>| <span data-ttu-id="9a9aa-117">Идентификатор проверенного издателя из учетной записи центра партнера издателя приложения.</span><span class="sxs-lookup"><span data-stu-id="9a9aa-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="9a9aa-118">аддеддатетиме</span><span class="sxs-lookup"><span data-stu-id="9a9aa-118">addedDateTime</span></span>|<span data-ttu-id="9a9aa-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="9a9aa-119">DateTimeOffSet</span></span>| <span data-ttu-id="9a9aa-120">Временная метка при первом добавлении проверенного издателя или последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="9a9aa-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9a9aa-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a9aa-121">JSON representation</span></span>
<span data-ttu-id="9a9aa-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a9aa-122">Here is a JSON representation of the resource.</span></span>

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
