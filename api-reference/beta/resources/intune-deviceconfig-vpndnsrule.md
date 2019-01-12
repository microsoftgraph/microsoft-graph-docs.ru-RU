---
title: Тип ресурса vpnDnsRule
description: Определение правила DNS VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3c928542f749973ac3abea041c8ca60ee74ff8fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964741"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="3e7b4-103">Тип ресурса vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="3e7b4-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="3e7b4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e7b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e7b4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e7b4-107">Определение правила DNS VPN.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="3e7b4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e7b4-108">Properties</span></span>
|<span data-ttu-id="3e7b4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e7b4-109">Property</span></span>|<span data-ttu-id="3e7b4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e7b4-110">Type</span></span>|<span data-ttu-id="3e7b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e7b4-112">name</span><span class="sxs-lookup"><span data-stu-id="3e7b4-112">name</span></span>|<span data-ttu-id="3e7b4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7b4-113">String</span></span>|<span data-ttu-id="3e7b4-114">Имя.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-114">Name.</span></span>|
|<span data-ttu-id="3e7b4-115">серверы</span><span class="sxs-lookup"><span data-stu-id="3e7b4-115">servers</span></span>|<span data-ttu-id="3e7b4-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e7b4-116">String collection</span></span>|<span data-ttu-id="3e7b4-117">Серверы.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-117">Servers.</span></span>|
|<span data-ttu-id="3e7b4-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="3e7b4-118">proxyServerUri</span></span>|<span data-ttu-id="3e7b4-119">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7b4-119">String</span></span>|<span data-ttu-id="3e7b4-120">Uri сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e7b4-121">Связи</span><span class="sxs-lookup"><span data-stu-id="3e7b4-121">Relationships</span></span>
<span data-ttu-id="3e7b4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3e7b4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e7b4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e7b4-123">JSON Representation</span></span>
<span data-ttu-id="3e7b4-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e7b4-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String"
}
```





