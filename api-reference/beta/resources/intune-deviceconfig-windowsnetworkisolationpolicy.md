---
title: Тип ресурса Виндовснетворкисолатионполици
description: Политика сетевой изоляции Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 78a598dab5c1eb003b09510f925506679bc432b3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293439"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="3201c-103">Тип ресурса Виндовснетворкисолатионполици</span><span class="sxs-lookup"><span data-stu-id="3201c-103">windowsNetworkIsolationPolicy resource type</span></span>

<span data-ttu-id="3201c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3201c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3201c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3201c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3201c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3201c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3201c-107">Политика сетевой изоляции Windows</span><span class="sxs-lookup"><span data-stu-id="3201c-107">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="3201c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3201c-108">Properties</span></span>
|<span data-ttu-id="3201c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3201c-109">Property</span></span>|<span data-ttu-id="3201c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3201c-110">Type</span></span>|<span data-ttu-id="3201c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3201c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3201c-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="3201c-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="3201c-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3201c-113">String collection</span></span>|<span data-ttu-id="3201c-114">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="3201c-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="3201c-115">Данные из одного из этих доменов, отправляемых на устройство, будут считаться корпоративными данными и защищены.</span><span class="sxs-lookup"><span data-stu-id="3201c-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="3201c-116">Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным.</span><span class="sxs-lookup"><span data-stu-id="3201c-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="3201c-117">Вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection</span><span class="sxs-lookup"><span data-stu-id="3201c-117">enterpriseCloudResources</span></span>|<span data-ttu-id="3201c-118">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="3201c-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="3201c-119">Содержит список корпоративных доменов ресурсов, размещенных в облаке и требующих защиты.</span><span class="sxs-lookup"><span data-stu-id="3201c-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="3201c-120">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="3201c-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="3201c-121">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="3201c-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="3201c-122">Прокси-сервер, используемый для этой цели, также должен быть настроен с использованием политики Ентерприсеинтерналпроксисерверс.</span><span class="sxs-lookup"><span data-stu-id="3201c-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="3201c-123">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3201c-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3201c-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="3201c-124">enterpriseIPRanges</span></span>|<span data-ttu-id="3201c-125">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="3201c-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="3201c-126">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="3201c-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="3201c-127">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="3201c-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="3201c-128">Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным.</span><span class="sxs-lookup"><span data-stu-id="3201c-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="3201c-129">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3201c-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3201c-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="3201c-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="3201c-131">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3201c-131">String collection</span></span>|<span data-ttu-id="3201c-132">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="3201c-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="3201c-133">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="3201c-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="3201c-134">Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="3201c-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="3201c-135">Они считаются корпоративными расположениями в сети.</span><span class="sxs-lookup"><span data-stu-id="3201c-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="3201c-136">Прокси-серверы используются только в настройке политики вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection для принудительного передачи трафика в соответствующие облачные ресурсы через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="3201c-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="3201c-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3201c-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="3201c-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="3201c-138">Boolean</span></span>|<span data-ttu-id="3201c-139">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="3201c-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="3201c-140">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="3201c-140">Default is false.</span></span>|
|<span data-ttu-id="3201c-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="3201c-141">enterpriseProxyServers</span></span>|<span data-ttu-id="3201c-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3201c-142">String collection</span></span>|<span data-ttu-id="3201c-143">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="3201c-143">This is a list of proxy servers.</span></span> <span data-ttu-id="3201c-144">Любой сервер, не включенный в этот список, считается не предприятием.</span><span class="sxs-lookup"><span data-stu-id="3201c-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="3201c-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3201c-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="3201c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3201c-146">Boolean</span></span>|<span data-ttu-id="3201c-147">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="3201c-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="3201c-148">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="3201c-148">Default is false</span></span>|
|<span data-ttu-id="3201c-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="3201c-149">neutralDomainResources</span></span>|<span data-ttu-id="3201c-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3201c-150">String collection</span></span>|<span data-ttu-id="3201c-151">Список доменных имен, которые могут использоваться для рабочего или личного ресурса.</span><span class="sxs-lookup"><span data-stu-id="3201c-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3201c-152">Связи</span><span class="sxs-lookup"><span data-stu-id="3201c-152">Relationships</span></span>
<span data-ttu-id="3201c-153">Нет</span><span class="sxs-lookup"><span data-stu-id="3201c-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3201c-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3201c-154">JSON Representation</span></span>
<span data-ttu-id="3201c-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3201c-155">Here is a JSON representation of the resource.</span></span>
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




