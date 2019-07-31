---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 36e46261c3f31d9d41a63097753799b634dadeb2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008721"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="43a3c-103">Тип ресурса Релатедконтакт</span><span class="sxs-lookup"><span data-stu-id="43a3c-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43a3c-104">Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет инфоратион для опекунов, возможностей, доктора и т. д.</span><span class="sxs-lookup"><span data-stu-id="43a3c-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides inforation for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="43a3c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="43a3c-105">Properties</span></span>
| <span data-ttu-id="43a3c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="43a3c-106">Property</span></span>     | <span data-ttu-id="43a3c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="43a3c-107">Type</span></span>   |<span data-ttu-id="43a3c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="43a3c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43a3c-109">id</span><span class="sxs-lookup"><span data-stu-id="43a3c-109">id</span></span>|<span data-ttu-id="43a3c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="43a3c-110">String</span></span>|<span data-ttu-id="43a3c-111">Идентификатор контакта в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="43a3c-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="43a3c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="43a3c-112">displayName</span></span>|<span data-ttu-id="43a3c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="43a3c-113">String</span></span>|<span data-ttu-id="43a3c-114">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="43a3c-114">Name of the contact.</span></span> <span data-ttu-id="43a3c-115">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="43a3c-115">Required.</span></span>|
|<span data-ttu-id="43a3c-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="43a3c-116">emailAddress</span></span>|<span data-ttu-id="43a3c-117">String</span><span class="sxs-lookup"><span data-stu-id="43a3c-117">String</span></span>|<span data-ttu-id="43a3c-118">Основной адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="43a3c-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="43a3c-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="43a3c-119">mobilePhone</span></span>|<span data-ttu-id="43a3c-120">String</span><span class="sxs-lookup"><span data-stu-id="43a3c-120">String</span></span>|<span data-ttu-id="43a3c-121">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="43a3c-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="43a3c-122">Отношение</span><span class="sxs-lookup"><span data-stu-id="43a3c-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="43a3c-123">Отношение к пользователю.</span><span class="sxs-lookup"><span data-stu-id="43a3c-123">Relationship to the user.</span></span> <span data-ttu-id="43a3c-124">Возможные значения: `parent`, `relative`, `aide`, `doctor` `guardian` `child`,,, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="43a3c-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="43a3c-125">Акцессконсент</span><span class="sxs-lookup"><span data-stu-id="43a3c-125">accessConsent</span></span>|<span data-ttu-id="43a3c-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="43a3c-126">Boolean</span></span>|<span data-ttu-id="43a3c-127">Указывает, было ли пользователь отправлен для доступа к данным учащихся.</span><span class="sxs-lookup"><span data-stu-id="43a3c-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43a3c-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43a3c-128">JSON representation</span></span>

<span data-ttu-id="43a3c-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43a3c-129">The following is a JSON representation of the resource.</span></span>

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
