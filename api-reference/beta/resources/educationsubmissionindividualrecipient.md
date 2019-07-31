---
title: Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент
description: 'Подкласс ЕдукатионсубмиссионреЦипиент, который указывает, что отправка назначена отдельному пользователю в классе.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2eecdc7e7ddd30ecad9a520b42cd11df9565fa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972511"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="01a34-103">Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="01a34-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01a34-104">Подкласс [едукатионсубмиссионреЦипиент](educationsubmissionrecipient.md) , который указывает, что отправка назначена отдельному пользователю в классе.</span><span class="sxs-lookup"><span data-stu-id="01a34-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="01a34-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="01a34-105">Properties</span></span>
| <span data-ttu-id="01a34-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="01a34-106">Property</span></span>     | <span data-ttu-id="01a34-107">Тип</span><span class="sxs-lookup"><span data-stu-id="01a34-107">Type</span></span>   |<span data-ttu-id="01a34-108">Описание</span><span class="sxs-lookup"><span data-stu-id="01a34-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01a34-109">userId</span><span class="sxs-lookup"><span data-stu-id="01a34-109">userId</span></span>|<span data-ttu-id="01a34-110">String</span><span class="sxs-lookup"><span data-stu-id="01a34-110">String</span></span>|<span data-ttu-id="01a34-111">Идентификатор пользователя, которому назначена отправка.</span><span class="sxs-lookup"><span data-stu-id="01a34-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01a34-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01a34-112">JSON representation</span></span>

<span data-ttu-id="01a34-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01a34-113">The following is a JSON representation of the resource.</span></span>

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
