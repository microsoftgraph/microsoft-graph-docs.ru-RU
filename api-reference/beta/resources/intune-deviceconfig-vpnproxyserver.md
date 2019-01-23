---
title: Тип ресурса vpnProxyServer
description: VPN-сервер прокси-сервера.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 676e56771f021a79179e268280f5e3190754eef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425675"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="8fcf2-103">Тип ресурса vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="8fcf2-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="8fcf2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8fcf2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fcf2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fcf2-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="8fcf2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fcf2-108">Properties</span></span>
|<span data-ttu-id="8fcf2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fcf2-109">Property</span></span>|<span data-ttu-id="8fcf2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8fcf2-110">Type</span></span>|<span data-ttu-id="8fcf2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8fcf2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fcf2-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="8fcf2-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="8fcf2-113">String</span><span class="sxs-lookup"><span data-stu-id="8fcf2-113">String</span></span>|<span data-ttu-id="8fcf2-114">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="8fcf2-115">address</span><span class="sxs-lookup"><span data-stu-id="8fcf2-115">address</span></span>|<span data-ttu-id="8fcf2-116">String</span><span class="sxs-lookup"><span data-stu-id="8fcf2-116">String</span></span>|<span data-ttu-id="8fcf2-117">Адрес.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-117">Address.</span></span>|
|<span data-ttu-id="8fcf2-118">port</span><span class="sxs-lookup"><span data-stu-id="8fcf2-118">port</span></span>|<span data-ttu-id="8fcf2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="8fcf2-119">Int32</span></span>|<span data-ttu-id="8fcf2-120">Порт.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-120">Port.</span></span> <span data-ttu-id="8fcf2-121">Допустимые значения от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="8fcf2-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fcf2-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="8fcf2-122">Relationships</span></span>
<span data-ttu-id="8fcf2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8fcf2-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fcf2-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fcf2-124">JSON Representation</span></span>
<span data-ttu-id="8fcf2-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fcf2-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```




