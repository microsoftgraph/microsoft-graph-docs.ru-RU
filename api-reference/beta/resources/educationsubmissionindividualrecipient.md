---
title: Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент
description: 'Подкласс ЕдукатионсубмиссионреЦипиент, который указывает, что отправка назначена отдельному пользователю в классе.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2954e511cee6929a66bb593c4f449f7410852c7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500725"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="6b2d0-103">Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="6b2d0-103">educationSubmissionIndividualRecipient resource type</span></span>

<span data-ttu-id="6b2d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b2d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b2d0-105">Подкласс [едукатионсубмиссионреЦипиент](educationsubmissionrecipient.md) , который указывает, что отправка назначена отдельному пользователю в классе.</span><span class="sxs-lookup"><span data-stu-id="6b2d0-105">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="6b2d0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b2d0-106">Properties</span></span>
| <span data-ttu-id="6b2d0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b2d0-107">Property</span></span>     | <span data-ttu-id="6b2d0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6b2d0-108">Type</span></span>   |<span data-ttu-id="6b2d0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6b2d0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b2d0-110">userId</span><span class="sxs-lookup"><span data-stu-id="6b2d0-110">userId</span></span>|<span data-ttu-id="6b2d0-111">String</span><span class="sxs-lookup"><span data-stu-id="6b2d0-111">String</span></span>|<span data-ttu-id="6b2d0-112">Идентификатор пользователя, которому назначена отправка.</span><span class="sxs-lookup"><span data-stu-id="6b2d0-112">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b2d0-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b2d0-113">JSON representation</span></span>

<span data-ttu-id="6b2d0-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b2d0-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
