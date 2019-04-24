---
title: Тип ресурса Секуритяктионстате
description: Представляет историю изменений состояния securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8f789dab438316f16b9c2607947fa08b7fcefdc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522022"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="8362d-103">Тип ресурса Секуритяктионстате</span><span class="sxs-lookup"><span data-stu-id="8362d-103">securityActionState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8362d-104">Представляет историю изменений состояния securityAction.</span><span class="sxs-lookup"><span data-stu-id="8362d-104">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="8362d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8362d-105">Properties</span></span>

| <span data-ttu-id="8362d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8362d-106">Property</span></span>     | <span data-ttu-id="8362d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8362d-107">Type</span></span>        | <span data-ttu-id="8362d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8362d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8362d-109">appId</span><span class="sxs-lookup"><span data-stu-id="8362d-109">appId</span></span>|<span data-ttu-id="8362d-110">String</span><span class="sxs-lookup"><span data-stu-id="8362d-110">String</span></span>|<span data-ttu-id="8362d-111">Идентификатор приложения вызывающего приложения, отправившего обновление (исправление) действию.</span><span class="sxs-lookup"><span data-stu-id="8362d-111">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="8362d-112">Его `appId` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="8362d-112">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="8362d-113">status</span><span class="sxs-lookup"><span data-stu-id="8362d-113">status</span></span>|<span data-ttu-id="8362d-114">String</span><span class="sxs-lookup"><span data-stu-id="8362d-114">String</span></span>| <span data-ttu-id="8362d-115">Состояние securityAction в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="8362d-115">Status of the securityAction in this update.</span></span> <span data-ttu-id="8362d-116">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="8362d-116">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="8362d-117">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="8362d-117">updatedDateTime</span></span>|<span data-ttu-id="8362d-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8362d-118">DateTimeOffset</span></span>| <span data-ttu-id="8362d-119">Временная метка при обновлении actionState.</span><span class="sxs-lookup"><span data-stu-id="8362d-119">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="8362d-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8362d-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8362d-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8362d-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8362d-122">user</span><span class="sxs-lookup"><span data-stu-id="8362d-122">user</span></span>|<span data-ttu-id="8362d-123">String</span><span class="sxs-lookup"><span data-stu-id="8362d-123">String</span></span>|<span data-ttu-id="8362d-124">Имя участника-пользователя, который выполнил вход в действие при отправке обновления (исправления).</span><span class="sxs-lookup"><span data-stu-id="8362d-124">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="8362d-125">Его `user` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="8362d-125">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8362d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8362d-126">JSON representation</span></span>

<span data-ttu-id="8362d-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8362d-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
