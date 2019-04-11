---
title: Тип ресурса Виндовснетворкисолатионполици
description: Политика сетевой изоляции Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b5e96a56f511289f75a7910f1defb44b7a20bf3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783551"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="6f75c-103">Тип ресурса Виндовснетворкисолатионполици</span><span class="sxs-lookup"><span data-stu-id="6f75c-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="6f75c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f75c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f75c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f75c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f75c-106">Политика сетевой изоляции Windows</span><span class="sxs-lookup"><span data-stu-id="6f75c-106">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="6f75c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f75c-107">Properties</span></span>
|<span data-ttu-id="6f75c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f75c-108">Property</span></span>|<span data-ttu-id="6f75c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f75c-109">Type</span></span>|<span data-ttu-id="6f75c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f75c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f75c-111">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="6f75c-111">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="6f75c-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f75c-112">String collection</span></span>|<span data-ttu-id="6f75c-113">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="6f75c-113">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="6f75c-114">Данные из одного из этих доменов, отправляемых на устройство, будут считаться корпоративными данными и защищены.</span><span class="sxs-lookup"><span data-stu-id="6f75c-114">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="6f75c-115">Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным.</span><span class="sxs-lookup"><span data-stu-id="6f75c-115">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="6f75c-116">Вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection</span><span class="sxs-lookup"><span data-stu-id="6f75c-116">enterpriseCloudResources</span></span>|<span data-ttu-id="6f75c-117">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="6f75c-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="6f75c-118">Содержит список корпоративных доменов ресурсов, размещенных в облаке и требующих защиты.</span><span class="sxs-lookup"><span data-stu-id="6f75c-118">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="6f75c-119">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="6f75c-119">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="6f75c-120">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="6f75c-120">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="6f75c-121">Прокси-сервер, используемый для этой цели, также должен быть настроен с использованием политики Ентерприсеинтерналпроксисерверс.</span><span class="sxs-lookup"><span data-stu-id="6f75c-121">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="6f75c-122">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6f75c-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6f75c-123">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="6f75c-123">enterpriseIPRanges</span></span>|<span data-ttu-id="6f75c-124">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6f75c-124">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="6f75c-125">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="6f75c-125">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="6f75c-126">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="6f75c-126">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="6f75c-127">Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным.</span><span class="sxs-lookup"><span data-stu-id="6f75c-127">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="6f75c-128">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6f75c-128">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6f75c-129">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="6f75c-129">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="6f75c-130">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f75c-130">String collection</span></span>|<span data-ttu-id="6f75c-131">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="6f75c-131">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="6f75c-132">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="6f75c-132">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="6f75c-133">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="6f75c-133">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="6f75c-134">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="6f75c-134">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="6f75c-135">Прокси-серверы используются только в настройке политики вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection для принудительного передачи трафика в соответствующие облачные ресурсы через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="6f75c-135">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="6f75c-136">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6f75c-136">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="6f75c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f75c-137">Boolean</span></span>|<span data-ttu-id="6f75c-138">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="6f75c-138">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="6f75c-139">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="6f75c-139">Default is false.</span></span>|
|<span data-ttu-id="6f75c-140">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="6f75c-140">enterpriseProxyServers</span></span>|<span data-ttu-id="6f75c-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f75c-141">String collection</span></span>|<span data-ttu-id="6f75c-142">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="6f75c-142">This is a list of proxy servers.</span></span> <span data-ttu-id="6f75c-143">Любой сервер, не включенный в этот список, считается не предприятием.</span><span class="sxs-lookup"><span data-stu-id="6f75c-143">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="6f75c-144">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="6f75c-144">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="6f75c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f75c-145">Boolean</span></span>|<span data-ttu-id="6f75c-146">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="6f75c-146">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="6f75c-147">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="6f75c-147">Default is false</span></span>|
|<span data-ttu-id="6f75c-148">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="6f75c-148">neutralDomainResources</span></span>|<span data-ttu-id="6f75c-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f75c-149">String collection</span></span>|<span data-ttu-id="6f75c-150">Список доменных имен, которые могут использоваться для рабочего или личного ресурса.</span><span class="sxs-lookup"><span data-stu-id="6f75c-150">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f75c-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="6f75c-151">Relationships</span></span>
<span data-ttu-id="6f75c-152">Нет</span><span class="sxs-lookup"><span data-stu-id="6f75c-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f75c-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f75c-153">JSON Representation</span></span>
<span data-ttu-id="6f75c-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f75c-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```





