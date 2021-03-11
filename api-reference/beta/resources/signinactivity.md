---
title: тип ресурса signInActivity
description: Предоставляет последнюю дату записи для определенного пользователя.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e48d2e64c71e67c623582552224a11636c7c6c7c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721861"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="9e454-103">тип ресурса signInActivity</span><span class="sxs-lookup"><span data-stu-id="9e454-103">signInActivity resource type</span></span>

<span data-ttu-id="9e454-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e454-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e454-105">Предоставляет дату последней записи для определенного [пользователя.](user.md)</span><span class="sxs-lookup"><span data-stu-id="9e454-105">Provides the last signed-in date for a specific [user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9e454-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e454-106">Properties</span></span>

| <span data-ttu-id="9e454-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e454-107">Property</span></span>     | <span data-ttu-id="9e454-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9e454-108">Type</span></span>        | <span data-ttu-id="9e454-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e454-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e454-110">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="9e454-110">lastSignInDateTime</span></span>|<span data-ttu-id="9e454-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e454-111">DateTimeOffset</span></span>|<span data-ttu-id="9e454-112">Последняя интерактивная дата регистрации для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e454-112">The last interactive sign-in date for a specific user.</span></span> <span data-ttu-id="9e454-113">Это поле можно использовать для вычисления последнего времени, когда пользователь вписался в каталог с помощью интерактивного метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9e454-113">You can use this field to calculate the last time a user signed in to the directory with an interactive authentication method.</span></span> <span data-ttu-id="9e454-114">Это поле можно использовать для создания отчетов, например неактивных пользователей.</span><span class="sxs-lookup"><span data-stu-id="9e454-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="9e454-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9e454-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e454-116">Например, полночь UTC 1 января 2014 г. : `'2014-01-01T00:00:00Z'` .</span><span class="sxs-lookup"><span data-stu-id="9e454-116">For example, midnight UTC on Jan 1, 2014 is: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9e454-117">Дополнительные сведения об использовании значения этого свойства см. в рубке Управление неактивными учетными записями пользователей [в Azure AD.](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="9e454-117">For more information about using the value of this property, see [Manage inactive user accounts in Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span></span>|
|<span data-ttu-id="9e454-118">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="9e454-118">lastSignInRequestId</span></span>|<span data-ttu-id="9e454-119">String</span><span class="sxs-lookup"><span data-stu-id="9e454-119">String</span></span>|<span data-ttu-id="9e454-120">Запрос ID последнего входного знака, выполненного этим пользователем.</span><span class="sxs-lookup"><span data-stu-id="9e454-120">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e454-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e454-121">JSON representation</span></span>

<span data-ttu-id="9e454-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e454-122">The following is a JSON representation of the resource.</span></span>

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
