---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a2e54e6d3c0ddea77758b083e5d2f979dc7f49b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526938"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="47f37-103">Тип ресурса Кустомсубжекталтернативенаме</span><span class="sxs-lookup"><span data-stu-id="47f37-103">customSubjectAlternativeName resource type</span></span>

<span data-ttu-id="47f37-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47f37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47f37-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47f37-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47f37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47f37-107">Определение альтернативного имени настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="47f37-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="47f37-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="47f37-108">Properties</span></span>
|<span data-ttu-id="47f37-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="47f37-109">Property</span></span>|<span data-ttu-id="47f37-110">Тип</span><span class="sxs-lookup"><span data-stu-id="47f37-110">Type</span></span>|<span data-ttu-id="47f37-111">Описание</span><span class="sxs-lookup"><span data-stu-id="47f37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47f37-112">сантипе</span><span class="sxs-lookup"><span data-stu-id="47f37-112">sanType</span></span>|[<span data-ttu-id="47f37-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="47f37-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="47f37-114">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="47f37-114">Custom SAN Type.</span></span> <span data-ttu-id="47f37-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="47f37-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="47f37-116">name</span><span class="sxs-lookup"><span data-stu-id="47f37-116">name</span></span>|<span data-ttu-id="47f37-117">String</span><span class="sxs-lookup"><span data-stu-id="47f37-117">String</span></span>|<span data-ttu-id="47f37-118">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="47f37-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="47f37-119">Связи</span><span class="sxs-lookup"><span data-stu-id="47f37-119">Relationships</span></span>
<span data-ttu-id="47f37-120">Нет</span><span class="sxs-lookup"><span data-stu-id="47f37-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47f37-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47f37-121">JSON Representation</span></span>
<span data-ttu-id="47f37-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47f37-122">Here is a JSON representation of the resource.</span></span>
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



