---
title: Тип ресурса vpnDnsRule
description: Определение правила DNS VPN.
ms.openlocfilehash: dcb6a0d3a0cd709e8a88835c553f9f29cb094e57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076576"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="78df6-103">Тип ресурса vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="78df6-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="78df6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78df6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78df6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78df6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78df6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78df6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78df6-107">Определение правила DNS VPN.</span><span class="sxs-lookup"><span data-stu-id="78df6-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="78df6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78df6-108">Properties</span></span>
|<span data-ttu-id="78df6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78df6-109">Property</span></span>|<span data-ttu-id="78df6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78df6-110">Type</span></span>|<span data-ttu-id="78df6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78df6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78df6-112">name</span><span class="sxs-lookup"><span data-stu-id="78df6-112">name</span></span>|<span data-ttu-id="78df6-113">String</span><span class="sxs-lookup"><span data-stu-id="78df6-113">String</span></span>|<span data-ttu-id="78df6-114">Имя.</span><span class="sxs-lookup"><span data-stu-id="78df6-114">Name.</span></span>|
|<span data-ttu-id="78df6-115">серверы</span><span class="sxs-lookup"><span data-stu-id="78df6-115">servers</span></span>|<span data-ttu-id="78df6-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="78df6-116">String collection</span></span>|<span data-ttu-id="78df6-117">Серверы.</span><span class="sxs-lookup"><span data-stu-id="78df6-117">Servers.</span></span>|
|<span data-ttu-id="78df6-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="78df6-118">proxyServerUri</span></span>|<span data-ttu-id="78df6-119">String</span><span class="sxs-lookup"><span data-stu-id="78df6-119">String</span></span>|<span data-ttu-id="78df6-120">Uri сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="78df6-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78df6-121">Связи</span><span class="sxs-lookup"><span data-stu-id="78df6-121">Relationships</span></span>
<span data-ttu-id="78df6-122">Нет</span><span class="sxs-lookup"><span data-stu-id="78df6-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78df6-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78df6-123">JSON Representation</span></span>
<span data-ttu-id="78df6-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78df6-124">Here is a JSON representation of the resource.</span></span>
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





