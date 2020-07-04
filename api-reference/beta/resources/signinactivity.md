---
title: Тип ресурса Сигнинактивити
description: Предоставляет дату последнего входа для определенного пользователя.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 385a4484090a58682fdd7560a7b7560a1601b124
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038672"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="b4d50-103">Тип ресурса Сигнинактивити</span><span class="sxs-lookup"><span data-stu-id="b4d50-103">signInActivity resource type</span></span>

<span data-ttu-id="b4d50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4d50-105">Предоставляет дату последнего входа для определенного [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="b4d50-105">Provides the last signed-in date for a specific [user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b4d50-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4d50-106">Properties</span></span>

| <span data-ttu-id="b4d50-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4d50-107">Property</span></span>     | <span data-ttu-id="b4d50-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b4d50-108">Type</span></span>        | <span data-ttu-id="b4d50-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b4d50-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4d50-110">ластсигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="b4d50-110">lastSignInDateTime</span></span>|<span data-ttu-id="b4d50-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4d50-111">DateTimeOffset</span></span>|<span data-ttu-id="b4d50-112">Дата последнего входа для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4d50-112">The last sign-in date for a specific user.</span></span> <span data-ttu-id="b4d50-113">С помощью этого поля можно вычислить время последнего входа пользователя в каталог.</span><span class="sxs-lookup"><span data-stu-id="b4d50-113">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="b4d50-114">Это поле можно использовать для создания отчетов, например неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="b4d50-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="b4d50-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b4d50-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b4d50-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b4d50-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b4d50-117">Дополнительные сведения об использовании значения этого свойства содержатся [в разделе Manage неактивных учетных записей пользователей в Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="b4d50-117">For more information about using the value of this property, see [Manage inactive user accounts in Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span></span>|
|<span data-ttu-id="b4d50-118">ластсигнинрекуестид</span><span class="sxs-lookup"><span data-stu-id="b4d50-118">lastSignInRequestId</span></span>|<span data-ttu-id="b4d50-119">String</span><span class="sxs-lookup"><span data-stu-id="b4d50-119">String</span></span>|<span data-ttu-id="b4d50-120">Идентификатор запроса последнего входа, выполненного этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="b4d50-120">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4d50-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b4d50-121">JSON representation</span></span>

<span data-ttu-id="b4d50-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4d50-122">The following is a JSON representation of the resource.</span></span>

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