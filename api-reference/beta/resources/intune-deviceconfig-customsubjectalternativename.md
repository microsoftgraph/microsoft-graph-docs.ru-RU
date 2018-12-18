---
title: Тип ресурса customSubjectAlternativeName
description: Настраиваемые определения имени субъекта
author: tfitzmac
ms.openlocfilehash: 5ed3f62cef38340ae7204b98e1fc984ba9bcb9cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349317"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="c2bf3-103">Тип ресурса customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="c2bf3-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="c2bf3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2bf3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2bf3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2bf3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2bf3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2bf3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2bf3-107">Настраиваемые определения имени субъекта</span><span class="sxs-lookup"><span data-stu-id="c2bf3-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="c2bf3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2bf3-108">Properties</span></span>
|<span data-ttu-id="c2bf3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2bf3-109">Property</span></span>|<span data-ttu-id="c2bf3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2bf3-110">Type</span></span>|<span data-ttu-id="c2bf3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2bf3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2bf3-112">sanType</span><span class="sxs-lookup"><span data-stu-id="c2bf3-112">sanType</span></span>|[<span data-ttu-id="c2bf3-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c2bf3-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c2bf3-114">Тип настраиваемого SAN.</span><span class="sxs-lookup"><span data-stu-id="c2bf3-114">Custom SAN Type.</span></span> <span data-ttu-id="c2bf3-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c2bf3-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c2bf3-116">name</span><span class="sxs-lookup"><span data-stu-id="c2bf3-116">name</span></span>|<span data-ttu-id="c2bf3-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c2bf3-117">String</span></span>|<span data-ttu-id="c2bf3-118">Имя настраиваемого SAN</span><span class="sxs-lookup"><span data-stu-id="c2bf3-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2bf3-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c2bf3-119">Relationships</span></span>
<span data-ttu-id="c2bf3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c2bf3-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2bf3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2bf3-121">JSON Representation</span></span>
<span data-ttu-id="c2bf3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2bf3-122">Here is a JSON representation of the resource.</span></span>
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





