---
title: Тип ресурса Сигнинактивити
description: Предоставляет дату последнего входа для определенного пользователя.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d93ff4f3b395d9b0820865c3293a419471ab6473
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939245"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="06140-103">Тип ресурса Сигнинактивити</span><span class="sxs-lookup"><span data-stu-id="06140-103">signInActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06140-104">Предоставляет дату последнего входа для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="06140-104">Provides the last signed-in date for a specific user.</span></span>

## <a name="properties"></a><span data-ttu-id="06140-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="06140-105">Properties</span></span>

| <span data-ttu-id="06140-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="06140-106">Property</span></span>     | <span data-ttu-id="06140-107">Тип</span><span class="sxs-lookup"><span data-stu-id="06140-107">Type</span></span>        | <span data-ttu-id="06140-108">Описание</span><span class="sxs-lookup"><span data-stu-id="06140-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="06140-109">ластсигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="06140-109">lastSignInDateTime</span></span>|<span data-ttu-id="06140-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06140-110">DateTimeOffset</span></span>|<span data-ttu-id="06140-111">Дата последнего входа для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="06140-111">The last sign-in date for a specific user.</span></span> <span data-ttu-id="06140-112">С помощью этого поля можно вычислить время последнего входа пользователя в каталог.</span><span class="sxs-lookup"><span data-stu-id="06140-112">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="06140-113">Это поле можно использовать для создания отчетов, например неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="06140-113">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="06140-114">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="06140-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="06140-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="06140-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="06140-116">ластсигнинрекуестид</span><span class="sxs-lookup"><span data-stu-id="06140-116">lastSignInRequestId</span></span>|<span data-ttu-id="06140-117">Строка</span><span class="sxs-lookup"><span data-stu-id="06140-117">String</span></span>|<span data-ttu-id="06140-118">Идентификатор запроса последнего входа, выполненного этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="06140-118">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06140-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06140-119">JSON representation</span></span>

<span data-ttu-id="06140-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06140-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->