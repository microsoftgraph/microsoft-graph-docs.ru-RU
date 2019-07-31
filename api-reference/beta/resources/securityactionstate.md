---
title: Тип ресурса Секуритяктионстате
description: Представляет историю изменений состояния securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e3efd29e156b6e0346574c74fad2a30a39ec7131
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008511"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="0d697-103">Тип ресурса Секуритяктионстате</span><span class="sxs-lookup"><span data-stu-id="0d697-103">securityActionState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d697-104">Представляет историю изменений состояния securityAction.</span><span class="sxs-lookup"><span data-stu-id="0d697-104">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="0d697-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d697-105">Properties</span></span>

| <span data-ttu-id="0d697-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d697-106">Property</span></span>     | <span data-ttu-id="0d697-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0d697-107">Type</span></span>        | <span data-ttu-id="0d697-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0d697-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d697-109">appId</span><span class="sxs-lookup"><span data-stu-id="0d697-109">appId</span></span>|<span data-ttu-id="0d697-110">String</span><span class="sxs-lookup"><span data-stu-id="0d697-110">String</span></span>|<span data-ttu-id="0d697-111">Идентификатор приложения вызывающего приложения, отправившего обновление (исправление) действию.</span><span class="sxs-lookup"><span data-stu-id="0d697-111">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="0d697-112">Его `appId` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="0d697-112">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="0d697-113">status</span><span class="sxs-lookup"><span data-stu-id="0d697-113">status</span></span>|<span data-ttu-id="0d697-114">String</span><span class="sxs-lookup"><span data-stu-id="0d697-114">String</span></span>| <span data-ttu-id="0d697-115">Состояние securityAction в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="0d697-115">Status of the securityAction in this update.</span></span> <span data-ttu-id="0d697-116">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="0d697-116">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="0d697-117">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="0d697-117">updatedDateTime</span></span>|<span data-ttu-id="0d697-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d697-118">DateTimeOffset</span></span>| <span data-ttu-id="0d697-119">Временная метка при обновлении actionState.</span><span class="sxs-lookup"><span data-stu-id="0d697-119">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="0d697-120">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0d697-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0d697-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0d697-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d697-122">user</span><span class="sxs-lookup"><span data-stu-id="0d697-122">user</span></span>|<span data-ttu-id="0d697-123">String</span><span class="sxs-lookup"><span data-stu-id="0d697-123">String</span></span>|<span data-ttu-id="0d697-124">Имя участника-пользователя, который выполнил вход в действие при отправке обновления (исправления).</span><span class="sxs-lookup"><span data-stu-id="0d697-124">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="0d697-125">Его `user` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="0d697-125">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d697-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d697-126">JSON representation</span></span>

<span data-ttu-id="0d697-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d697-127">The following is a JSON representation of the resource.</span></span>

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
