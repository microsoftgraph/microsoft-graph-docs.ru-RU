---
title: Тип ресурса vpnDnsRule
description: Определение правила DNS VPN.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d09e26b105a139f04db34ba69184fcf60e9ef238
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868203"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="5f0e7-103">Тип ресурса vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="5f0e7-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="5f0e7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f0e7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f0e7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f0e7-107">Определение правила DNS VPN.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="5f0e7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f0e7-108">Properties</span></span>
|<span data-ttu-id="5f0e7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f0e7-109">Property</span></span>|<span data-ttu-id="5f0e7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5f0e7-110">Type</span></span>|<span data-ttu-id="5f0e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5f0e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f0e7-112">name</span><span class="sxs-lookup"><span data-stu-id="5f0e7-112">name</span></span>|<span data-ttu-id="5f0e7-113">Строка</span><span class="sxs-lookup"><span data-stu-id="5f0e7-113">String</span></span>|<span data-ttu-id="5f0e7-114">Имя.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-114">Name.</span></span>|
|<span data-ttu-id="5f0e7-115">серверы</span><span class="sxs-lookup"><span data-stu-id="5f0e7-115">servers</span></span>|<span data-ttu-id="5f0e7-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5f0e7-116">String collection</span></span>|<span data-ttu-id="5f0e7-117">Серверы.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-117">Servers.</span></span>|
|<span data-ttu-id="5f0e7-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="5f0e7-118">proxyServerUri</span></span>|<span data-ttu-id="5f0e7-119">Строка</span><span class="sxs-lookup"><span data-stu-id="5f0e7-119">String</span></span>|<span data-ttu-id="5f0e7-120">Uri сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f0e7-121">Связи</span><span class="sxs-lookup"><span data-stu-id="5f0e7-121">Relationships</span></span>
<span data-ttu-id="5f0e7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5f0e7-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f0e7-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f0e7-123">JSON Representation</span></span>
<span data-ttu-id="5f0e7-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f0e7-124">Here is a JSON representation of the resource.</span></span>
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





