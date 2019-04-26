---
title: Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент
description: 'Подкласс ЕдукатионсубмиссионреЦипиент, который указывает, что отправка назначена отдельному пользователю в классе.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: de58dc743cd50f0e31021b4651bb0a3b3b192197
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340558"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="00076-103">Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент</span><span class="sxs-lookup"><span data-stu-id="00076-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00076-104">Подкласс [едукатионсубмиссионреЦипиент](educationsubmissionrecipient.md) , который указывает, что отправка назначена отдельному пользователю в классе.</span><span class="sxs-lookup"><span data-stu-id="00076-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="00076-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="00076-105">Properties</span></span>
| <span data-ttu-id="00076-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="00076-106">Property</span></span>     | <span data-ttu-id="00076-107">Тип</span><span class="sxs-lookup"><span data-stu-id="00076-107">Type</span></span>   |<span data-ttu-id="00076-108">Описание</span><span class="sxs-lookup"><span data-stu-id="00076-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00076-109">userId</span><span class="sxs-lookup"><span data-stu-id="00076-109">userId</span></span>|<span data-ttu-id="00076-110">String</span><span class="sxs-lookup"><span data-stu-id="00076-110">String</span></span>|<span data-ttu-id="00076-111">Идентификатор пользователя, которому назначена отправка.</span><span class="sxs-lookup"><span data-stu-id="00076-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00076-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00076-112">JSON representation</span></span>

<span data-ttu-id="00076-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00076-113">The following is a JSON representation of the resource.</span></span>

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
