---
title: тип ресурса educationOnPremisesInfo
description: Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4c5da3180b1c15f2363bfd651d0f4e3d68f41b60
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232262"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="7de6b-103">тип ресурса educationOnPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="7de6b-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="7de6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de6b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7de6b-105">Дополнительные сведения, используемые для связываия локальной учетной записи пользователя Active Directory с объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7de6b-105">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="7de6b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7de6b-106">Properties</span></span>

| <span data-ttu-id="7de6b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7de6b-107">Property</span></span>    | <span data-ttu-id="7de6b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7de6b-108">Type</span></span>   | <span data-ttu-id="7de6b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7de6b-109">Description</span></span>                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| <span data-ttu-id="7de6b-110">immutableId</span><span class="sxs-lookup"><span data-stu-id="7de6b-110">immutableId</span></span> | <span data-ttu-id="7de6b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="7de6b-111">String</span></span> | <span data-ttu-id="7de6b-112">Уникальный идентификатор объекта пользователя в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7de6b-112">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7de6b-113">Связи</span><span class="sxs-lookup"><span data-stu-id="7de6b-113">Relationships</span></span>

<span data-ttu-id="7de6b-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7de6b-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7de6b-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7de6b-115">JSON representation</span></span>

<span data-ttu-id="7de6b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7de6b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOnPremisesInfo",
  "immutableId": "String"
}
```
