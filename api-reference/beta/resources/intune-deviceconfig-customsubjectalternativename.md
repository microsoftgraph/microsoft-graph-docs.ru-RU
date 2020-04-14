---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b88b5c6a393d994de5d393984ee339969b25ba6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453466"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="94d7e-103">Тип ресурса Кустомсубжекталтернативенаме</span><span class="sxs-lookup"><span data-stu-id="94d7e-103">customSubjectAlternativeName resource type</span></span>

<span data-ttu-id="94d7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94d7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94d7e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94d7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94d7e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94d7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94d7e-107">Определение альтернативного имени настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="94d7e-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="94d7e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="94d7e-108">Properties</span></span>
|<span data-ttu-id="94d7e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="94d7e-109">Property</span></span>|<span data-ttu-id="94d7e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="94d7e-110">Type</span></span>|<span data-ttu-id="94d7e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="94d7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94d7e-112">сантипе</span><span class="sxs-lookup"><span data-stu-id="94d7e-112">sanType</span></span>|[<span data-ttu-id="94d7e-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="94d7e-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="94d7e-114">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="94d7e-114">Custom SAN Type.</span></span> <span data-ttu-id="94d7e-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="94d7e-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="94d7e-116">name</span><span class="sxs-lookup"><span data-stu-id="94d7e-116">name</span></span>|<span data-ttu-id="94d7e-117">String</span><span class="sxs-lookup"><span data-stu-id="94d7e-117">String</span></span>|<span data-ttu-id="94d7e-118">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="94d7e-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="94d7e-119">Связи</span><span class="sxs-lookup"><span data-stu-id="94d7e-119">Relationships</span></span>
<span data-ttu-id="94d7e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="94d7e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94d7e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94d7e-121">JSON Representation</span></span>
<span data-ttu-id="94d7e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94d7e-122">Here is a JSON representation of the resource.</span></span>
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



