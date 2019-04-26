---
title: Тип ресурса Релатедконтакт
description: Контактная запись, связанная с educationUser, которая предоставляет информацию для хранителя, возможностей, доктора и т. д.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563066"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="3d583-103">Тип ресурса Релатедконтакт</span><span class="sxs-lookup"><span data-stu-id="3d583-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d583-104">Контактная запись, связанная с [educationUser](../resources/educationuser.md) , которая предоставляет инфоратион для опекунов, возможностей, доктора и т. д.</span><span class="sxs-lookup"><span data-stu-id="3d583-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides inforation for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="3d583-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d583-105">Properties</span></span>
| <span data-ttu-id="3d583-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d583-106">Property</span></span>     | <span data-ttu-id="3d583-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3d583-107">Type</span></span>   |<span data-ttu-id="3d583-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3d583-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d583-109">id</span><span class="sxs-lookup"><span data-stu-id="3d583-109">id</span></span>|<span data-ttu-id="3d583-110">Строка</span><span class="sxs-lookup"><span data-stu-id="3d583-110">String</span></span>|<span data-ttu-id="3d583-111">Идентификатор контакта в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d583-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="3d583-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3d583-112">displayName</span></span>|<span data-ttu-id="3d583-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3d583-113">String</span></span>|<span data-ttu-id="3d583-114">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="3d583-114">Name of the contact.</span></span> <span data-ttu-id="3d583-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d583-115">Required.</span></span>|
|<span data-ttu-id="3d583-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3d583-116">emailAddress</span></span>|<span data-ttu-id="3d583-117">String</span><span class="sxs-lookup"><span data-stu-id="3d583-117">String</span></span>|<span data-ttu-id="3d583-118">Основной адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="3d583-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="3d583-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="3d583-119">mobilePhone</span></span>|<span data-ttu-id="3d583-120">String</span><span class="sxs-lookup"><span data-stu-id="3d583-120">String</span></span>|<span data-ttu-id="3d583-121">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="3d583-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="3d583-122">Отношение</span><span class="sxs-lookup"><span data-stu-id="3d583-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="3d583-123">Отношение к пользователю.</span><span class="sxs-lookup"><span data-stu-id="3d583-123">Relationship to the user.</span></span> <span data-ttu-id="3d583-124">Возможные значения: `parent`, `relative`, `aide`, `doctor` `guardian` `child`,,, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3d583-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3d583-125">Акцессконсент</span><span class="sxs-lookup"><span data-stu-id="3d583-125">accessConsent</span></span>|<span data-ttu-id="3d583-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d583-126">Boolean</span></span>|<span data-ttu-id="3d583-127">Указывает, было ли пользователь отправлен для доступа к данным учащихся.</span><span class="sxs-lookup"><span data-stu-id="3d583-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d583-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d583-128">JSON representation</span></span>

<span data-ttu-id="3d583-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d583-129">The following is a JSON representation of the resource.</span></span>

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
