---
title: Тип ресурса Организатионсеттингс
description: Содержит параметры, которые применяются к организациям или объектам пользователей в ней.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 80b7272915cd6f9dbfc381aa93a32896e2eaf3f5
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051049"
---
# <a name="organizationsettings-resource-type"></a><span data-ttu-id="5a447-103">Тип ресурса Организатионсеттингс</span><span class="sxs-lookup"><span data-stu-id="5a447-103">organizationSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a447-104">Содержит параметры, применимые к [Организации](organization.md) или применяемые к объектам [пользователей](user.md) в Организации.</span><span class="sxs-lookup"><span data-stu-id="5a447-104">Contains settings that are applicable to the [organization](organization.md) or that should be applied to [user](user.md) objects within an organization.</span></span>

## <a name="methods"></a><span data-ttu-id="5a447-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5a447-105">Methods</span></span>

| <span data-ttu-id="5a447-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5a447-106">Method</span></span>       | <span data-ttu-id="5a447-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a447-107">Return Type</span></span> | <span data-ttu-id="5a447-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5a447-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5a447-109">Получение параметров Организации</span><span class="sxs-lookup"><span data-stu-id="5a447-109">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="5a447-110">организатионсеттингс</span><span class="sxs-lookup"><span data-stu-id="5a447-110">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="5a447-111">Чтение объекта параметров Организации.</span><span class="sxs-lookup"><span data-stu-id="5a447-111">Read the organization settings object.</span></span> |
| [<span data-ttu-id="5a447-112">Создание Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="5a447-112">Create profileCardProperty</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="5a447-113">профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="5a447-113">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="5a447-114">Создание нового Профилекардпроперти путем отправки в коллекцию Профилекардпропертиес.</span><span class="sxs-lookup"><span data-stu-id="5a447-114">Create a new profileCardProperty by posting to the profileCardProperties collection.</span></span> |
| [<span data-ttu-id="5a447-115">Список Профилекардпропертиес</span><span class="sxs-lookup"><span data-stu-id="5a447-115">List profileCardProperties</span></span>](../api/organizationsettings-list-profilecardproperties.md) | <span data-ttu-id="5a447-116">Коллекция [профилекардпроперти](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5a447-116">[profileCardProperty](profilecardproperty.md) collection</span></span> | <span data-ttu-id="5a447-117">Получение коллекции объектов Профилекардпроперти.</span><span class="sxs-lookup"><span data-stu-id="5a447-117">Get a profileCardProperty object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a447-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a447-118">Properties</span></span>

<span data-ttu-id="5a447-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5a447-119">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="5a447-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5a447-120">Relationships</span></span>

| <span data-ttu-id="5a447-121">Связь</span><span class="sxs-lookup"><span data-stu-id="5a447-121">Relationship</span></span> | <span data-ttu-id="5a447-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5a447-122">Type</span></span>        | <span data-ttu-id="5a447-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5a447-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a447-124">id</span><span class="sxs-lookup"><span data-stu-id="5a447-124">id</span></span> |<span data-ttu-id="5a447-125">String</span><span class="sxs-lookup"><span data-stu-id="5a447-125">String</span></span>| <span data-ttu-id="5a447-126">Идентификатор объекта параметров для Организации.</span><span class="sxs-lookup"><span data-stu-id="5a447-126">Id of the settings object for the organization.</span></span> |
|<span data-ttu-id="5a447-127">профилекардпропертиес</span><span class="sxs-lookup"><span data-stu-id="5a447-127">profileCardProperties</span></span>|<span data-ttu-id="5a447-128">Коллекция [профилекардпроперти](profilecardproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5a447-128">[profileCardProperty](profilecardproperty.md) collection</span></span>| <span data-ttu-id="5a447-129">Содержит коллекцию свойств, которые администратор определил как видимый в карточке профиля M365.</span><span class="sxs-lookup"><span data-stu-id="5a447-129">Contains a collection of the properties an administrator has defined as visible on the M365 Profile Card.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a447-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5a447-130">JSON representation</span></span>

<span data-ttu-id="5a447-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a447-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
