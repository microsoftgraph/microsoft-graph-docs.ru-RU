---
title: Тип ресурса customSubjectAlternativeName
description: Настраиваемые определения имени субъекта
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 069cc1f6d93c785e4fc774d7988e0fc80febbb12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954122"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="52980-103">Тип ресурса customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="52980-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="52980-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="52980-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52980-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52980-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52980-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="52980-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52980-107">Настраиваемые определения имени субъекта</span><span class="sxs-lookup"><span data-stu-id="52980-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="52980-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="52980-108">Properties</span></span>
|<span data-ttu-id="52980-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="52980-109">Property</span></span>|<span data-ttu-id="52980-110">Тип</span><span class="sxs-lookup"><span data-stu-id="52980-110">Type</span></span>|<span data-ttu-id="52980-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52980-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52980-112">sanType</span><span class="sxs-lookup"><span data-stu-id="52980-112">sanType</span></span>|[<span data-ttu-id="52980-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="52980-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="52980-114">Тип настраиваемого SAN.</span><span class="sxs-lookup"><span data-stu-id="52980-114">Custom SAN Type.</span></span> <span data-ttu-id="52980-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="52980-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="52980-116">name</span><span class="sxs-lookup"><span data-stu-id="52980-116">name</span></span>|<span data-ttu-id="52980-117">Строка</span><span class="sxs-lookup"><span data-stu-id="52980-117">String</span></span>|<span data-ttu-id="52980-118">Имя настраиваемого SAN</span><span class="sxs-lookup"><span data-stu-id="52980-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="52980-119">Связи</span><span class="sxs-lookup"><span data-stu-id="52980-119">Relationships</span></span>
<span data-ttu-id="52980-120">Нет</span><span class="sxs-lookup"><span data-stu-id="52980-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52980-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52980-121">JSON Representation</span></span>
<span data-ttu-id="52980-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52980-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





