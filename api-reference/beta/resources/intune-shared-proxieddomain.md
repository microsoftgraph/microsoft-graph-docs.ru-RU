---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
ms.openlocfilehash: d00dc72d7a7156fb90cbeee914c157f446dda81a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341988"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="78b46-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="78b46-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="78b46-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78b46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78b46-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78b46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78b46-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78b46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78b46-107">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="78b46-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="78b46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78b46-108">Properties</span></span>
|<span data-ttu-id="78b46-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78b46-109">Property</span></span>|<span data-ttu-id="78b46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78b46-110">Type</span></span>|<span data-ttu-id="78b46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78b46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78b46-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="78b46-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="78b46-113">Строка</span><span class="sxs-lookup"><span data-stu-id="78b46-113">String</span></span>|<span data-ttu-id="78b46-114">IP-адрес или полное доменное имя (FQDN).</span><span class="sxs-lookup"><span data-stu-id="78b46-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="78b46-115">proxy</span><span class="sxs-lookup"><span data-stu-id="78b46-115">proxy</span></span>|<span data-ttu-id="78b46-116">Строка</span><span class="sxs-lookup"><span data-stu-id="78b46-116">String</span></span>|<span data-ttu-id="78b46-117">IP-адрес прокси-сервера или полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="78b46-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78b46-118">Связи</span><span class="sxs-lookup"><span data-stu-id="78b46-118">Relationships</span></span>
<span data-ttu-id="78b46-119">Нет</span><span class="sxs-lookup"><span data-stu-id="78b46-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78b46-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78b46-120">JSON Representation</span></span>
<span data-ttu-id="78b46-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78b46-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



