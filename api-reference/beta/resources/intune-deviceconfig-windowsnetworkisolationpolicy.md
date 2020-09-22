---
title: Тип ресурса Виндовснетворкисолатионполици
description: Политика сетевой изоляции Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60ffe01d03c3c32ec9d051498905cca98e3cbd12
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061842"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="65f31-103">Тип ресурса Виндовснетворкисолатионполици</span><span class="sxs-lookup"><span data-stu-id="65f31-103">windowsNetworkIsolationPolicy resource type</span></span>

<span data-ttu-id="65f31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65f31-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f31-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65f31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f31-107">Политика сетевой изоляции Windows</span><span class="sxs-lookup"><span data-stu-id="65f31-107">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="65f31-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="65f31-108">Properties</span></span>
|<span data-ttu-id="65f31-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="65f31-109">Property</span></span>|<span data-ttu-id="65f31-110">Тип</span><span class="sxs-lookup"><span data-stu-id="65f31-110">Type</span></span>|<span data-ttu-id="65f31-111">Описание</span><span class="sxs-lookup"><span data-stu-id="65f31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f31-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="65f31-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="65f31-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="65f31-113">String collection</span></span>|<span data-ttu-id="65f31-114">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="65f31-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="65f31-115">Данные из одного из этих доменов, отправляемых на устройство, будут считаться корпоративными данными и защищены.</span><span class="sxs-lookup"><span data-stu-id="65f31-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="65f31-116">Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным.</span><span class="sxs-lookup"><span data-stu-id="65f31-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="65f31-117">Вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection</span><span class="sxs-lookup"><span data-stu-id="65f31-117">enterpriseCloudResources</span></span>|<span data-ttu-id="65f31-118">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="65f31-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="65f31-119">Содержит список корпоративных доменов ресурсов, размещенных в облаке и требующих защиты.</span><span class="sxs-lookup"><span data-stu-id="65f31-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="65f31-120">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="65f31-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="65f31-121">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="65f31-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="65f31-122">Прокси-сервер, используемый для этой цели, также должен быть настроен с использованием политики Ентерприсеинтерналпроксисерверс.</span><span class="sxs-lookup"><span data-stu-id="65f31-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="65f31-123">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="65f31-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="65f31-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="65f31-124">enterpriseIPRanges</span></span>|<span data-ttu-id="65f31-125">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="65f31-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="65f31-126">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="65f31-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="65f31-127">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="65f31-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="65f31-128">Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным.</span><span class="sxs-lookup"><span data-stu-id="65f31-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="65f31-129">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="65f31-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="65f31-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="65f31-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="65f31-131">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="65f31-131">String collection</span></span>|<span data-ttu-id="65f31-132">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="65f31-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="65f31-133">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="65f31-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="65f31-134">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="65f31-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="65f31-135">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="65f31-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="65f31-136">Прокси-серверы используются только в настройке политики вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection для принудительного передачи трафика в соответствующие облачные ресурсы через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="65f31-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="65f31-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="65f31-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="65f31-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f31-138">Boolean</span></span>|<span data-ttu-id="65f31-139">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="65f31-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="65f31-140">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="65f31-140">Default is false.</span></span>|
|<span data-ttu-id="65f31-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="65f31-141">enterpriseProxyServers</span></span>|<span data-ttu-id="65f31-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="65f31-142">String collection</span></span>|<span data-ttu-id="65f31-143">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="65f31-143">This is a list of proxy servers.</span></span> <span data-ttu-id="65f31-144">Любой сервер, не включенный в этот список, считается не предприятием.</span><span class="sxs-lookup"><span data-stu-id="65f31-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="65f31-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="65f31-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="65f31-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f31-146">Boolean</span></span>|<span data-ttu-id="65f31-147">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="65f31-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="65f31-148">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="65f31-148">Default is false</span></span>|
|<span data-ttu-id="65f31-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="65f31-149">neutralDomainResources</span></span>|<span data-ttu-id="65f31-150">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="65f31-150">String collection</span></span>|<span data-ttu-id="65f31-151">Список доменных имен, которые могут использоваться для рабочего или личного ресурса.</span><span class="sxs-lookup"><span data-stu-id="65f31-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65f31-152">Связи</span><span class="sxs-lookup"><span data-stu-id="65f31-152">Relationships</span></span>
<span data-ttu-id="65f31-153">Нет</span><span class="sxs-lookup"><span data-stu-id="65f31-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65f31-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65f31-154">JSON Representation</span></span>
<span data-ttu-id="65f31-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65f31-155">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange"
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






