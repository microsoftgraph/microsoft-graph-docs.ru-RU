---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 93069c2f9f2aa46c5d6d0f2f992762efab062064
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533862"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="925f9-103">Тип ресурса Реалтедконтакт</span><span class="sxs-lookup"><span data-stu-id="925f9-103">realtedContact resource type</span></span>

<span data-ttu-id="925f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="925f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="925f9-105">Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет информацию для хранителя, возможностей, доктора и т. д.</span><span class="sxs-lookup"><span data-stu-id="925f9-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="925f9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="925f9-106">Properties</span></span>
| <span data-ttu-id="925f9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="925f9-107">Property</span></span>     | <span data-ttu-id="925f9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="925f9-108">Type</span></span>   |<span data-ttu-id="925f9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="925f9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="925f9-110">id</span><span class="sxs-lookup"><span data-stu-id="925f9-110">id</span></span>|<span data-ttu-id="925f9-111">Строка</span><span class="sxs-lookup"><span data-stu-id="925f9-111">String</span></span>|<span data-ttu-id="925f9-112">Идентификатор контакта в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="925f9-112">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="925f9-113">displayName</span><span class="sxs-lookup"><span data-stu-id="925f9-113">displayName</span></span>|<span data-ttu-id="925f9-114">Строка</span><span class="sxs-lookup"><span data-stu-id="925f9-114">String</span></span>|<span data-ttu-id="925f9-115">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="925f9-115">Name of the contact.</span></span> <span data-ttu-id="925f9-116">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="925f9-116">Required.</span></span>|
|<span data-ttu-id="925f9-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="925f9-117">emailAddress</span></span>|<span data-ttu-id="925f9-118">String</span><span class="sxs-lookup"><span data-stu-id="925f9-118">String</span></span>|<span data-ttu-id="925f9-119">Основной адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="925f9-119">Primary email address of the contact.</span></span>|
|<span data-ttu-id="925f9-120">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="925f9-120">mobilePhone</span></span>|<span data-ttu-id="925f9-121">String</span><span class="sxs-lookup"><span data-stu-id="925f9-121">String</span></span>|<span data-ttu-id="925f9-122">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="925f9-122">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="925f9-123">Отношение</span><span class="sxs-lookup"><span data-stu-id="925f9-123">relationship</span></span>|`contactRelationship`|<span data-ttu-id="925f9-124">Отношение к пользователю.</span><span class="sxs-lookup"><span data-stu-id="925f9-124">Relationship to the user.</span></span> <span data-ttu-id="925f9-125">Возможные значения: `parent`, `relative`, `aide`, `doctor` `guardian` `child`,,, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="925f9-125">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="925f9-126">акцессконсент</span><span class="sxs-lookup"><span data-stu-id="925f9-126">accessConsent</span></span>|<span data-ttu-id="925f9-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="925f9-127">Boolean</span></span>|<span data-ttu-id="925f9-128">Указывает, было ли пользователь отправлен для доступа к данным учащихся.</span><span class="sxs-lookup"><span data-stu-id="925f9-128">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="925f9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="925f9-129">JSON representation</span></span>

<span data-ttu-id="925f9-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="925f9-130">The following is a JSON representation of the resource.</span></span>

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
