---
title: Тип ресурса customSubjectAlternativeName
description: Настраиваемые определения имени субъекта
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3f081b37b79be45d6705d24be58ea7295b58b68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415672"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="2b15f-103">Тип ресурса customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="2b15f-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="2b15f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b15f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b15f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b15f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b15f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b15f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b15f-107">Настраиваемые определения имени субъекта</span><span class="sxs-lookup"><span data-stu-id="2b15f-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="2b15f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b15f-108">Properties</span></span>
|<span data-ttu-id="2b15f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b15f-109">Property</span></span>|<span data-ttu-id="2b15f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2b15f-110">Type</span></span>|<span data-ttu-id="2b15f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2b15f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b15f-112">sanType</span><span class="sxs-lookup"><span data-stu-id="2b15f-112">sanType</span></span>|[<span data-ttu-id="2b15f-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2b15f-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="2b15f-114">Тип настраиваемого SAN.</span><span class="sxs-lookup"><span data-stu-id="2b15f-114">Custom SAN Type.</span></span> <span data-ttu-id="2b15f-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="2b15f-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="2b15f-116">name</span><span class="sxs-lookup"><span data-stu-id="2b15f-116">name</span></span>|<span data-ttu-id="2b15f-117">String</span><span class="sxs-lookup"><span data-stu-id="2b15f-117">String</span></span>|<span data-ttu-id="2b15f-118">Имя настраиваемого SAN</span><span class="sxs-lookup"><span data-stu-id="2b15f-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b15f-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="2b15f-119">Relationships</span></span>
<span data-ttu-id="2b15f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2b15f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b15f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b15f-121">JSON Representation</span></span>
<span data-ttu-id="2b15f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b15f-122">Here is a JSON representation of the resource.</span></span>
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




