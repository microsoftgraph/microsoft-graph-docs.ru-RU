---
title: тип ресурсов relatedContact
description: Запись контактов, связанная с educationUser, который предоставляет информацию для опекунов, помощников, врачей и так далее.
author: mmast-msft
ms.author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37c494d58896af34c1da12e6e500a0561d877911
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960336"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="82b16-103">тип ресурсов relatedContact</span><span class="sxs-lookup"><span data-stu-id="82b16-103">relatedContact resource type</span></span>

<span data-ttu-id="82b16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82b16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82b16-105">Запись контактов, связанная с [educationUser,](../resources/educationuser.md) который предоставляет информацию для опекунов, помощников, врачей и так далее.</span><span class="sxs-lookup"><span data-stu-id="82b16-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="82b16-106">Методы</span><span class="sxs-lookup"><span data-stu-id="82b16-106">Methods</span></span>

| <span data-ttu-id="82b16-107">Метод</span><span class="sxs-lookup"><span data-stu-id="82b16-107">Method</span></span>                                    | <span data-ttu-id="82b16-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="82b16-108">Return Type</span></span>                   | <span data-ttu-id="82b16-109">Описание</span><span class="sxs-lookup"><span data-stu-id="82b16-109">Description</span></span>                                                             |
| :---------------------------------------- | :---------------------------- | :---------------------------------------------------------------------- |
| [<span data-ttu-id="82b16-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="82b16-110">Update</span></span>](../api/relatedcontact-update.md) | <span data-ttu-id="82b16-111">**коллекция relatedContact**</span><span class="sxs-lookup"><span data-stu-id="82b16-111">**relatedContact** collection</span></span> | <span data-ttu-id="82b16-112">Обновление **связанныхContacts** для [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="82b16-112">Update the **relatedContacts** for an [educationUser](educationuser.md)</span></span> |

## <a name="properties"></a><span data-ttu-id="82b16-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="82b16-113">Properties</span></span>

| <span data-ttu-id="82b16-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="82b16-114">Property</span></span>      | <span data-ttu-id="82b16-115">Тип</span><span class="sxs-lookup"><span data-stu-id="82b16-115">Type</span></span>                | <span data-ttu-id="82b16-116">Описание</span><span class="sxs-lookup"><span data-stu-id="82b16-116">Description</span></span>                                                                                                                                |
| :------------ | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="82b16-117">displayName</span><span class="sxs-lookup"><span data-stu-id="82b16-117">displayName</span></span>   | <span data-ttu-id="82b16-118">Строка</span><span class="sxs-lookup"><span data-stu-id="82b16-118">String</span></span>              | <span data-ttu-id="82b16-119">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="82b16-119">Name of the contact.</span></span> <span data-ttu-id="82b16-120">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82b16-120">Required.</span></span>                                                                                                             |
| <span data-ttu-id="82b16-121">accessConsent</span><span class="sxs-lookup"><span data-stu-id="82b16-121">accessConsent</span></span> | <span data-ttu-id="82b16-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b16-122">Boolean</span></span>             | <span data-ttu-id="82b16-123">Указывает, было ли получено согласие пользователя на доступ к данным учащихся.</span><span class="sxs-lookup"><span data-stu-id="82b16-123">Indicates whether the user has been consented to access student data.</span></span>                                                                      |
| <span data-ttu-id="82b16-124">emailAddress</span><span class="sxs-lookup"><span data-stu-id="82b16-124">emailAddress</span></span>  | <span data-ttu-id="82b16-125">String</span><span class="sxs-lookup"><span data-stu-id="82b16-125">String</span></span>              | <span data-ttu-id="82b16-126">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="82b16-126">Email address of the contact.</span></span>                                                                                                              |
| <span data-ttu-id="82b16-127">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="82b16-127">mobilePhone</span></span>   | <span data-ttu-id="82b16-128">String</span><span class="sxs-lookup"><span data-stu-id="82b16-128">String</span></span>              | <span data-ttu-id="82b16-129">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="82b16-129">Mobile phone number of the contact.</span></span>                                                                                                        |
| <span data-ttu-id="82b16-130">Отношение</span><span class="sxs-lookup"><span data-stu-id="82b16-130">relationship</span></span>  | <span data-ttu-id="82b16-131">contactRelationship</span><span class="sxs-lookup"><span data-stu-id="82b16-131">contactRelationship</span></span> | <span data-ttu-id="82b16-132">Отношение к пользователю.</span><span class="sxs-lookup"><span data-stu-id="82b16-132">Relationship to the user.</span></span> <span data-ttu-id="82b16-133">Возможные значения: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="82b16-133">Possible values are: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="82b16-134">Связи</span><span class="sxs-lookup"><span data-stu-id="82b16-134">Relationships</span></span>

<span data-ttu-id="82b16-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="82b16-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82b16-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="82b16-136">JSON representation</span></span>

<span data-ttu-id="82b16-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82b16-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": "Boolean"
}
```
