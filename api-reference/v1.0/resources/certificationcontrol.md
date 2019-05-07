---
title: Тип ресурса Цертификатионконтрол
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: c92d129b6849898abe7202b9c2f539f26d2e1ebe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629315"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="fa44d-103">Тип ресурса Цертификатионконтрол</span><span class="sxs-lookup"><span data-stu-id="fa44d-103">certificationControl resource type</span></span>

<span data-ttu-id="fa44d-104">Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.</span><span class="sxs-lookup"><span data-stu-id="fa44d-104">Contains compliance certification data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="fa44d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa44d-105">Properties</span></span>

|<span data-ttu-id="fa44d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa44d-106">Property</span></span> |<span data-ttu-id="fa44d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fa44d-107">Type</span></span> |<span data-ttu-id="fa44d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fa44d-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="fa44d-109">name</span><span class="sxs-lookup"><span data-stu-id="fa44d-109">name</span></span>|<span data-ttu-id="fa44d-110">String</span><span class="sxs-lookup"><span data-stu-id="fa44d-110">String</span></span>|<span data-ttu-id="fa44d-111">Имя элемента управления сертификацией</span><span class="sxs-lookup"><span data-stu-id="fa44d-111">Certification control name</span></span> |
|<span data-ttu-id="fa44d-112">url</span><span class="sxs-lookup"><span data-stu-id="fa44d-112">url</span></span>|<span data-ttu-id="fa44d-113">String</span><span class="sxs-lookup"><span data-stu-id="fa44d-113">String</span></span>|<span data-ttu-id="fa44d-114">URL-адрес портала доверия службы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="fa44d-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa44d-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fa44d-115">JSON representation</span></span>

<span data-ttu-id="fa44d-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa44d-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
