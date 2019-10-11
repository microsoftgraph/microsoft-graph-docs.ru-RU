---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ce1ff84abb6704255267b521c67e5fc7b231b7df
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439936"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="adb2a-103">Тип ресурса Релатедконтакт</span><span class="sxs-lookup"><span data-stu-id="adb2a-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adb2a-104">Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет информацию для хранителя, возможностей, доктора и т. д.</span><span class="sxs-lookup"><span data-stu-id="adb2a-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="adb2a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="adb2a-105">Properties</span></span>

| <span data-ttu-id="adb2a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="adb2a-106">Property</span></span>      | <span data-ttu-id="adb2a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="adb2a-107">Type</span></span>                  | <span data-ttu-id="adb2a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="adb2a-108">Description</span></span>                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="adb2a-109">id</span><span class="sxs-lookup"><span data-stu-id="adb2a-109">id</span></span>            | <span data-ttu-id="adb2a-110">Строка</span><span class="sxs-lookup"><span data-stu-id="adb2a-110">String</span></span>                | <span data-ttu-id="adb2a-111">Идентификатор контакта в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="adb2a-111">Identity of the contact within Azure Active Directory.</span></span>                                                              |
| <span data-ttu-id="adb2a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="adb2a-112">displayName</span></span>   | <span data-ttu-id="adb2a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="adb2a-113">String</span></span>                | <span data-ttu-id="adb2a-114">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="adb2a-114">Name of the contact.</span></span> <span data-ttu-id="adb2a-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adb2a-115">Required.</span></span>                                                                                      |
| <span data-ttu-id="adb2a-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="adb2a-116">emailAddress</span></span>  | <span data-ttu-id="adb2a-117">String</span><span class="sxs-lookup"><span data-stu-id="adb2a-117">String</span></span>                | <span data-ttu-id="adb2a-118">Основной адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="adb2a-118">Primary email address of the contact.</span></span>                                                                               |
| <span data-ttu-id="adb2a-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="adb2a-119">mobilePhone</span></span>   | <span data-ttu-id="adb2a-120">String</span><span class="sxs-lookup"><span data-stu-id="adb2a-120">String</span></span>                | <span data-ttu-id="adb2a-121">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="adb2a-121">Mobile phone number of the contact.</span></span>                                                                                 |
| <span data-ttu-id="adb2a-122">Отношение</span><span class="sxs-lookup"><span data-stu-id="adb2a-122">relationship</span></span>  | `contactRelationship` | <span data-ttu-id="adb2a-123">Отношение к пользователю.</span><span class="sxs-lookup"><span data-stu-id="adb2a-123">Relationship to the user.</span></span> <span data-ttu-id="adb2a-124">Возможные значения: `parent`, `relative`, `aide`, `doctor` `guardian`,, `child`, `other`.</span><span class="sxs-lookup"><span data-stu-id="adb2a-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`.</span></span> |
| <span data-ttu-id="adb2a-125">акцессконсент</span><span class="sxs-lookup"><span data-stu-id="adb2a-125">accessConsent</span></span> | <span data-ttu-id="adb2a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="adb2a-126">Boolean</span></span>               | <span data-ttu-id="adb2a-127">Указывает, было ли пользователь отправлен для доступа к данным учащихся.</span><span class="sxs-lookup"><span data-stu-id="adb2a-127">Indicates whether the user has been consented to access student data.</span></span>                                               |

## <a name="json-representation"></a><span data-ttu-id="adb2a-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="adb2a-128">JSON representation</span></span>

<span data-ttu-id="adb2a-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adb2a-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
