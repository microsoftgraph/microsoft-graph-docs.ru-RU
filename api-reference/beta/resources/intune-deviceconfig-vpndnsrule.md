---
title: Тип ресурса vpnDnsRule
description: Определение правила DNS VPN.
author: tfitzmac
ms.openlocfilehash: 7be94c48dafd4352938ac2c63ab1af66c65ea098
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351165"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="717a4-103">Тип ресурса vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="717a4-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="717a4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="717a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="717a4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="717a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="717a4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="717a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="717a4-107">Определение правила DNS VPN.</span><span class="sxs-lookup"><span data-stu-id="717a4-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="717a4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="717a4-108">Properties</span></span>
|<span data-ttu-id="717a4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="717a4-109">Property</span></span>|<span data-ttu-id="717a4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="717a4-110">Type</span></span>|<span data-ttu-id="717a4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="717a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="717a4-112">name</span><span class="sxs-lookup"><span data-stu-id="717a4-112">name</span></span>|<span data-ttu-id="717a4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="717a4-113">String</span></span>|<span data-ttu-id="717a4-114">Имя.</span><span class="sxs-lookup"><span data-stu-id="717a4-114">Name.</span></span>|
|<span data-ttu-id="717a4-115">серверы</span><span class="sxs-lookup"><span data-stu-id="717a4-115">servers</span></span>|<span data-ttu-id="717a4-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="717a4-116">String collection</span></span>|<span data-ttu-id="717a4-117">Серверы.</span><span class="sxs-lookup"><span data-stu-id="717a4-117">Servers.</span></span>|
|<span data-ttu-id="717a4-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="717a4-118">proxyServerUri</span></span>|<span data-ttu-id="717a4-119">String.</span><span class="sxs-lookup"><span data-stu-id="717a4-119">String</span></span>|<span data-ttu-id="717a4-120">Uri сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="717a4-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="717a4-121">Связи</span><span class="sxs-lookup"><span data-stu-id="717a4-121">Relationships</span></span>
<span data-ttu-id="717a4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="717a4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="717a4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="717a4-123">JSON Representation</span></span>
<span data-ttu-id="717a4-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="717a4-124">Here is a JSON representation of the resource.</span></span>
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





