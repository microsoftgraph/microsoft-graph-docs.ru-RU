---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 22f28942f891bc8ac72f6640091e0b8e1195f51f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795654"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="dffea-103">Тип ресурса Кустомсубжекталтернативенаме</span><span class="sxs-lookup"><span data-stu-id="dffea-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="dffea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dffea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dffea-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dffea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dffea-106">Определение альтернативного имени настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="dffea-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="dffea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dffea-107">Properties</span></span>
|<span data-ttu-id="dffea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dffea-108">Property</span></span>|<span data-ttu-id="dffea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dffea-109">Type</span></span>|<span data-ttu-id="dffea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dffea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dffea-111">сантипе</span><span class="sxs-lookup"><span data-stu-id="dffea-111">sanType</span></span>|[<span data-ttu-id="dffea-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="dffea-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="dffea-113">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="dffea-113">Custom SAN Type.</span></span> <span data-ttu-id="dffea-114">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="dffea-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="dffea-115">name</span><span class="sxs-lookup"><span data-stu-id="dffea-115">name</span></span>|<span data-ttu-id="dffea-116">String</span><span class="sxs-lookup"><span data-stu-id="dffea-116">String</span></span>|<span data-ttu-id="dffea-117">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="dffea-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="dffea-118">Связи</span><span class="sxs-lookup"><span data-stu-id="dffea-118">Relationships</span></span>
<span data-ttu-id="dffea-119">Нет</span><span class="sxs-lookup"><span data-stu-id="dffea-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dffea-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dffea-120">JSON Representation</span></span>
<span data-ttu-id="dffea-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dffea-121">Here is a JSON representation of the resource.</span></span>
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



