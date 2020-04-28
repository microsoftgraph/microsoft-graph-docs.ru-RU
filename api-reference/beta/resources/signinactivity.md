---
title: Тип ресурса Сигнинактивити
description: Предоставляет дату последнего входа для определенного пользователя.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 86678b346466caa5c0d7a139a6da9ce0cf09e0c0
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125297"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="d4bf8-103">Тип ресурса Сигнинактивити</span><span class="sxs-lookup"><span data-stu-id="d4bf8-103">signInActivity resource type</span></span>

<span data-ttu-id="d4bf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4bf8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4bf8-105">Предоставляет дату последнего входа для определенного [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="d4bf8-105">Provides the last signed-in date for a specific [user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d4bf8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4bf8-106">Properties</span></span>

| <span data-ttu-id="d4bf8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4bf8-107">Property</span></span>     | <span data-ttu-id="d4bf8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d4bf8-108">Type</span></span>        | <span data-ttu-id="d4bf8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d4bf8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4bf8-110">ластсигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="d4bf8-110">lastSignInDateTime</span></span>|<span data-ttu-id="d4bf8-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4bf8-111">DateTimeOffset</span></span>|<span data-ttu-id="d4bf8-112">Дата последнего входа для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4bf8-112">The last sign-in date for a specific user.</span></span> <span data-ttu-id="d4bf8-113">С помощью этого поля можно вычислить время последнего входа пользователя в каталог.</span><span class="sxs-lookup"><span data-stu-id="d4bf8-113">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="d4bf8-114">Это поле можно использовать для создания отчетов, например неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="d4bf8-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="d4bf8-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d4bf8-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d4bf8-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d4bf8-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d4bf8-117">ластсигнинрекуестид</span><span class="sxs-lookup"><span data-stu-id="d4bf8-117">lastSignInRequestId</span></span>|<span data-ttu-id="d4bf8-118">String</span><span class="sxs-lookup"><span data-stu-id="d4bf8-118">String</span></span>|<span data-ttu-id="d4bf8-119">Идентификатор запроса последнего входа, выполненного этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="d4bf8-119">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4bf8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4bf8-120">JSON representation</span></span>

<span data-ttu-id="d4bf8-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4bf8-121">The following is a JSON representation of the resource.</span></span>

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