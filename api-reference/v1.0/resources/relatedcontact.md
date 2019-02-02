---
title: Тип ресурса relatedContact
description: Запись контакта, связанные с educationUser, который предоставляет сведения для опекунов, возможностей, врачи и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694491"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="35638-103">Тип ресурса realtedContact</span><span class="sxs-lookup"><span data-stu-id="35638-103">realtedContact resource type</span></span>

<span data-ttu-id="35638-104">Запись контакта, связанные с [educationUser](../resources/educationuser.md) , который предоставляет сведения для опекунов, возможностей, врачи и т. д.</span><span class="sxs-lookup"><span data-stu-id="35638-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="35638-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="35638-105">Properties</span></span>
| <span data-ttu-id="35638-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="35638-106">Property</span></span>     | <span data-ttu-id="35638-107">Тип</span><span class="sxs-lookup"><span data-stu-id="35638-107">Type</span></span>   |<span data-ttu-id="35638-108">Описание</span><span class="sxs-lookup"><span data-stu-id="35638-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35638-109">id</span><span class="sxs-lookup"><span data-stu-id="35638-109">id</span></span>|<span data-ttu-id="35638-110">Строка</span><span class="sxs-lookup"><span data-stu-id="35638-110">String</span></span>|<span data-ttu-id="35638-111">Идентификатор контакта в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="35638-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="35638-112">displayName</span><span class="sxs-lookup"><span data-stu-id="35638-112">displayName</span></span>|<span data-ttu-id="35638-113">String</span><span class="sxs-lookup"><span data-stu-id="35638-113">String</span></span>|<span data-ttu-id="35638-114">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="35638-114">Name of the contact.</span></span> <span data-ttu-id="35638-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35638-115">Required.</span></span>|
|<span data-ttu-id="35638-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="35638-116">emailAddress</span></span>|<span data-ttu-id="35638-117">String</span><span class="sxs-lookup"><span data-stu-id="35638-117">String</span></span>|<span data-ttu-id="35638-118">Основной адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="35638-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="35638-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="35638-119">mobilePhone</span></span>|<span data-ttu-id="35638-120">String</span><span class="sxs-lookup"><span data-stu-id="35638-120">String</span></span>|<span data-ttu-id="35638-121">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="35638-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="35638-122">Отношение</span><span class="sxs-lookup"><span data-stu-id="35638-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="35638-123">Отношение к пользователю.</span><span class="sxs-lookup"><span data-stu-id="35638-123">Relationship to the user.</span></span> <span data-ttu-id="35638-124">Возможные значения: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="35638-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="35638-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="35638-125">accessConsent</span></span>|<span data-ttu-id="35638-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="35638-126">Boolean</span></span>|<span data-ttu-id="35638-127">Указывает, был ли пользователь изъявил для доступа к данным учебы.</span><span class="sxs-lookup"><span data-stu-id="35638-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35638-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35638-128">JSON representation</span></span>

<span data-ttu-id="35638-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35638-129">The following is a JSON representation of the resource.</span></span>

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
