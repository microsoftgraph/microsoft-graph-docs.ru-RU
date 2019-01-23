---
title: Тип ресурса windowsNetworkIsolationPolicy
description: Политики изоляции сети Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c7ab7addffa4ff3f9b84ced60c30fe8707c695b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403758"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="3ebaf-103">Тип ресурса windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="3ebaf-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="3ebaf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ebaf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ebaf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ebaf-107">Политики изоляции сети Windows</span><span class="sxs-lookup"><span data-stu-id="3ebaf-107">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="3ebaf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ebaf-108">Properties</span></span>
|<span data-ttu-id="3ebaf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ebaf-109">Property</span></span>|<span data-ttu-id="3ebaf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3ebaf-110">Type</span></span>|<span data-ttu-id="3ebaf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3ebaf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ebaf-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="3ebaf-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="3ebaf-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ebaf-113">String collection</span></span>|<span data-ttu-id="3ebaf-114">Это список доменов, входящих в границы предприятия.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="3ebaf-115">Данные из одного из этих доменов, которые отправлены на устройство будет считаться корпоративных данных и защищенные.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="3ebaf-116">Безопасные место назначения для корпоративных данных открыть общий доступ в будут считаться местоположениях.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="3ebaf-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="3ebaf-117">enterpriseCloudResources</span></span>|<span data-ttu-id="3ebaf-118">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="3ebaf-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="3ebaf-119">Содержит список доменов ресурсов предприятия, размещенные в облаке, должны быть защищены.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="3ebaf-120">Подключения к этим ресурсам считаются корпоративными данными.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="3ebaf-121">Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80).</span><span class="sxs-lookup"><span data-stu-id="3ebaf-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="3ebaf-122">Для этой цели использовать прокси-сервер должен быть настроен с помощью политики EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="3ebaf-123">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3ebaf-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="3ebaf-124">enterpriseIPRanges</span></span>|<span data-ttu-id="3ebaf-125">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="3ebaf-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="3ebaf-126">Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="3ebaf-127">Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="3ebaf-128">Безопасные место назначения для корпоративных данных открыть общий доступ в будут считаться местоположениях.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="3ebaf-129">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3ebaf-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="3ebaf-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="3ebaf-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ebaf-131">String collection</span></span>|<span data-ttu-id="3ebaf-132">Это список внутренних прокси-серверов, разделенных запятыми</span><span class="sxs-lookup"><span data-stu-id="3ebaf-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="3ebaf-133">(например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59").</span><span class="sxs-lookup"><span data-stu-id="3ebaf-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="3ebaf-134">Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="3ebaf-135">Они считаются корпоративными серверами.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="3ebaf-136">Прокси-серверов только выполнять во время настройки EnterpriseCloudResources политики для принудительного трафика совпавших облачных ресурсов через эти прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="3ebaf-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3ebaf-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="3ebaf-138">Логический</span><span class="sxs-lookup"><span data-stu-id="3ebaf-138">Boolean</span></span>|<span data-ttu-id="3ebaf-139">Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="3ebaf-140">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-140">Default is false.</span></span>|
|<span data-ttu-id="3ebaf-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="3ebaf-141">enterpriseProxyServers</span></span>|<span data-ttu-id="3ebaf-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ebaf-142">String collection</span></span>|<span data-ttu-id="3ebaf-143">Это список прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-143">This is a list of proxy servers.</span></span> <span data-ttu-id="3ebaf-144">Любой сервер не в этом списке считается вне предприятия.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="3ebaf-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="3ebaf-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="3ebaf-146">Логический</span><span class="sxs-lookup"><span data-stu-id="3ebaf-146">Boolean</span></span>|<span data-ttu-id="3ebaf-147">Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="3ebaf-148">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-148">Default is false</span></span>|
|<span data-ttu-id="3ebaf-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="3ebaf-149">neutralDomainResources</span></span>|<span data-ttu-id="3ebaf-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ebaf-150">String collection</span></span>|<span data-ttu-id="3ebaf-151">Список имен доменов, которые можно использовать для рабочих или личных ресурса.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ebaf-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ebaf-152">Relationships</span></span>
<span data-ttu-id="3ebaf-153">Нет</span><span class="sxs-lookup"><span data-stu-id="3ebaf-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ebaf-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ebaf-154">JSON Representation</span></span>
<span data-ttu-id="3ebaf-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ebaf-155">Here is a JSON representation of the resource.</span></span>
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




