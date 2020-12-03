---
title: Тип ресурса Сигнинактивити
description: Предоставляет дату последнего входа для определенного пользователя.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e8300e787fe516a9712359f99ebf215f4813a0b9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521231"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="b86dd-103">Тип ресурса Сигнинактивити</span><span class="sxs-lookup"><span data-stu-id="b86dd-103">signInActivity resource type</span></span>

<span data-ttu-id="b86dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b86dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b86dd-105">Предоставляет дату последнего входа для определенного [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="b86dd-105">Provides the last signed-in date for a specific [user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b86dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b86dd-106">Properties</span></span>

| <span data-ttu-id="b86dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b86dd-107">Property</span></span>     | <span data-ttu-id="b86dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b86dd-108">Type</span></span>        | <span data-ttu-id="b86dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b86dd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b86dd-110">ластсигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="b86dd-110">lastSignInDateTime</span></span>|<span data-ttu-id="b86dd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b86dd-111">DateTimeOffset</span></span>|<span data-ttu-id="b86dd-112">Дата последнего входа для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b86dd-112">The last sign-in date for a specific user.</span></span> <span data-ttu-id="b86dd-113">С помощью этого поля можно вычислить время последнего входа пользователя в каталог.</span><span class="sxs-lookup"><span data-stu-id="b86dd-113">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="b86dd-114">Это поле можно использовать для создания отчетов, например неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="b86dd-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="b86dd-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b86dd-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b86dd-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b86dd-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b86dd-117">Дополнительные сведения об использовании значения этого свойства содержатся [в разделе Manage неактивных учетных записей пользователей в Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="b86dd-117">For more information about using the value of this property, see [Manage inactive user accounts in Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span></span>|
|<span data-ttu-id="b86dd-118">ластсигнинрекуестид</span><span class="sxs-lookup"><span data-stu-id="b86dd-118">lastSignInRequestId</span></span>|<span data-ttu-id="b86dd-119">String</span><span class="sxs-lookup"><span data-stu-id="b86dd-119">String</span></span>|<span data-ttu-id="b86dd-120">Идентификатор запроса последнего входа, выполненного этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="b86dd-120">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b86dd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b86dd-121">JSON representation</span></span>

<span data-ttu-id="b86dd-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b86dd-122">The following is a JSON representation of the resource.</span></span>

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