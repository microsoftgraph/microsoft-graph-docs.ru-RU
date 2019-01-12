---
title: Тип ресурса embeddedSIMActivationCode
description: Встроенный код активации диспетчера установки как предоставленный оператором мобильной.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af8bf020953dbc014f42aa6d363d3ca9e30db8a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987407"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="8b4b1-103">Тип ресурса embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="8b4b1-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="8b4b1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b4b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b4b1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b4b1-107">Встроенный код активации диспетчера установки как предоставленный оператором мобильной.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="8b4b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b4b1-108">Properties</span></span>
|<span data-ttu-id="8b4b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b4b1-109">Property</span></span>|<span data-ttu-id="8b4b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8b4b1-110">Type</span></span>|<span data-ttu-id="8b4b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8b4b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b4b1-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="8b4b1-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="8b4b1-113">Строка</span><span class="sxs-lookup"><span data-stu-id="8b4b1-113">String</span></span>|<span data-ttu-id="8b4b1-114">Идентификатор карточки интегральной (ICCID) для данного встроенного кода активации диспетчера установки, предоставленный оператор мобильной связи.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="8b4b1-115">Входные данные должно соответствовать следующим регулярным выражением: "^\[0-9\]{19}\[0-9\]?$".</span><span class="sxs-lookup"><span data-stu-id="8b4b1-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="8b4b1-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="8b4b1-116">matchingIdentifier</span></span>|<span data-ttu-id="8b4b1-117">Строка</span><span class="sxs-lookup"><span data-stu-id="8b4b1-117">String</span></span>|<span data-ttu-id="8b4b1-118">MatchingIdentifier (MatchingID), указанный в GSMA связь SGP.22 Отклика технические спецификации раздел 4.1.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="8b4b1-119">Входные данные должно соответствовать следующим регулярным выражением: "^\[a-zA-Z0-9\-\]\* $".</span><span class="sxs-lookup"><span data-stu-id="8b4b1-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="8b4b1-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="8b4b1-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="8b4b1-121">Строка</span><span class="sxs-lookup"><span data-stu-id="8b4b1-121">String</span></span>|<span data-ttu-id="8b4b1-122">Полное доменное имя SM-DP + server технические спецификации Отклика SPG связи GSM.22.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="8b4b1-123">Входные данные должно соответствовать следующим регулярным выражением: "^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$".</span><span class="sxs-lookup"><span data-stu-id="8b4b1-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b4b1-124">Связи</span><span class="sxs-lookup"><span data-stu-id="8b4b1-124">Relationships</span></span>
<span data-ttu-id="8b4b1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="8b4b1-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b4b1-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b4b1-126">JSON Representation</span></span>
<span data-ttu-id="8b4b1-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b4b1-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```





