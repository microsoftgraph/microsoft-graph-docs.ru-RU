---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: adea95729dd4e6558885223245a7225811f14677
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002949"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="6a34c-103">Тип ресурса Реалтедконтакт</span><span class="sxs-lookup"><span data-stu-id="6a34c-103">realtedContact resource type</span></span>

<span data-ttu-id="6a34c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a34c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a34c-105">Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет информацию для хранителя, возможностей, доктора и т. д.</span><span class="sxs-lookup"><span data-stu-id="6a34c-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="6a34c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a34c-106">Properties</span></span>

| <span data-ttu-id="6a34c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a34c-107">Property</span></span>      | <span data-ttu-id="6a34c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6a34c-108">Type</span></span>                  | <span data-ttu-id="6a34c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6a34c-109">Description</span></span>                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6a34c-110">id</span><span class="sxs-lookup"><span data-stu-id="6a34c-110">id</span></span>            | <span data-ttu-id="6a34c-111">String</span><span class="sxs-lookup"><span data-stu-id="6a34c-111">String</span></span>                | <span data-ttu-id="6a34c-112">Идентификатор контакта в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6a34c-112">Identity of the contact within Azure Active Directory.</span></span>                                                                                    |
| <span data-ttu-id="6a34c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6a34c-113">displayName</span></span>   | <span data-ttu-id="6a34c-114">String</span><span class="sxs-lookup"><span data-stu-id="6a34c-114">String</span></span>                | <span data-ttu-id="6a34c-115">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="6a34c-115">Name of the contact.</span></span> <span data-ttu-id="6a34c-116">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6a34c-116">Required.</span></span>                                                                                                            |
| <span data-ttu-id="6a34c-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6a34c-117">emailAddress</span></span>  | <span data-ttu-id="6a34c-118">String</span><span class="sxs-lookup"><span data-stu-id="6a34c-118">String</span></span>                | <span data-ttu-id="6a34c-119">Основной адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="6a34c-119">Primary email address of the contact.</span></span>                                                                                                     |
| <span data-ttu-id="6a34c-120">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="6a34c-120">mobilePhone</span></span>   | <span data-ttu-id="6a34c-121">String</span><span class="sxs-lookup"><span data-stu-id="6a34c-121">String</span></span>                | <span data-ttu-id="6a34c-122">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="6a34c-122">Mobile phone number of the contact.</span></span>                                                                                                       |
| <span data-ttu-id="6a34c-123">Отношение</span><span class="sxs-lookup"><span data-stu-id="6a34c-123">relationship</span></span>  | `contactRelationship` | <span data-ttu-id="6a34c-124">Отношение к пользователю.</span><span class="sxs-lookup"><span data-stu-id="6a34c-124">Relationship to the user.</span></span> <span data-ttu-id="6a34c-125">Возможные значения:,,,,,, `parent` `relative` `aide` `doctor` `guardian` `child` `other` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="6a34c-125">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="6a34c-126">акцессконсент</span><span class="sxs-lookup"><span data-stu-id="6a34c-126">accessConsent</span></span> | <span data-ttu-id="6a34c-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a34c-127">Boolean</span></span>               | <span data-ttu-id="6a34c-128">Указывает, было ли пользователь отправлен для доступа к данным учащихся.</span><span class="sxs-lookup"><span data-stu-id="6a34c-128">Indicates whether the user has been consented to access student data.</span></span>                                                                     |

## <a name="json-representation"></a><span data-ttu-id="6a34c-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a34c-129">JSON representation</span></span>

<span data-ttu-id="6a34c-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a34c-130">The following is a JSON representation of the resource.</span></span>

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

