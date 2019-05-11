---
title: Тип ресурса Виндовсфиреваллруле
description: Правило, контролирующее трафик через брандмауэр Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbf322718bd3b95e27583350bf840cc05f2e6ca0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944063"
---
# <a name="windowsfirewallrule-resource-type"></a><span data-ttu-id="367fb-103">Тип ресурса Виндовсфиреваллруле</span><span class="sxs-lookup"><span data-stu-id="367fb-103">windowsFirewallRule resource type</span></span>

> <span data-ttu-id="367fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="367fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="367fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="367fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="367fb-106">Правило, контролирующее трафик через брандмауэр Windows.</span><span class="sxs-lookup"><span data-stu-id="367fb-106">A rule controlling traffic through the Windows Firewall.</span></span>

## <a name="properties"></a><span data-ttu-id="367fb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="367fb-107">Properties</span></span>
|<span data-ttu-id="367fb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="367fb-108">Property</span></span>|<span data-ttu-id="367fb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="367fb-109">Type</span></span>|<span data-ttu-id="367fb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="367fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="367fb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="367fb-111">displayName</span></span>|<span data-ttu-id="367fb-112">Строка</span><span class="sxs-lookup"><span data-stu-id="367fb-112">String</span></span>|<span data-ttu-id="367fb-113">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="367fb-113">The display name of the rule.</span></span> <span data-ttu-id="367fb-114">Не обязательно должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="367fb-114">Does not need to be unique.</span></span>|
|<span data-ttu-id="367fb-115">description</span><span class="sxs-lookup"><span data-stu-id="367fb-115">description</span></span>|<span data-ttu-id="367fb-116">String</span><span class="sxs-lookup"><span data-stu-id="367fb-116">String</span></span>|<span data-ttu-id="367fb-117">Описание правила.</span><span class="sxs-lookup"><span data-stu-id="367fb-117">The description of the rule.</span></span>|
|<span data-ttu-id="367fb-118">Паккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="367fb-118">packageFamilyName</span></span>|<span data-ttu-id="367fb-119">Строка</span><span class="sxs-lookup"><span data-stu-id="367fb-119">String</span></span>|<span data-ttu-id="367fb-120">Имя семейства пакетов приложения Microsoft Store, на которое влияет правило брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="367fb-120">The package family name of a Microsoft Store application that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="367fb-121">Пути</span><span class="sxs-lookup"><span data-stu-id="367fb-121">filePath</span></span>|<span data-ttu-id="367fb-122">Строка</span><span class="sxs-lookup"><span data-stu-id="367fb-122">String</span></span>|<span data-ttu-id="367fb-123">Полный путь к файлу приложения, на который влияет правило брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="367fb-123">The full file path of an app that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="367fb-124">Служба</span><span class="sxs-lookup"><span data-stu-id="367fb-124">serviceName</span></span>|<span data-ttu-id="367fb-125">Строка</span><span class="sxs-lookup"><span data-stu-id="367fb-125">String</span></span>|<span data-ttu-id="367fb-126">Имя, используемое в случаях, когда служба, а не приложение, отправляет или получает трафик.</span><span class="sxs-lookup"><span data-stu-id="367fb-126">The name used in cases when a service, not an application, is sending or receiving traffic.</span></span>|
|<span data-ttu-id="367fb-127">Protocol</span><span class="sxs-lookup"><span data-stu-id="367fb-127">protocol</span></span>|<span data-ttu-id="367fb-128">Int32</span><span class="sxs-lookup"><span data-stu-id="367fb-128">Int32</span></span>|<span data-ttu-id="367fb-129">0-255 число, представляющее протокол IP (TCP = 6, UDP = 17).</span><span class="sxs-lookup"><span data-stu-id="367fb-129">0-255 number representing the IP protocol (TCP = 6, UDP = 17).</span></span> <span data-ttu-id="367fb-130">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="367fb-130">If not specified, the default is All.</span></span> <span data-ttu-id="367fb-131">Допустимые значения — от 0 до 255</span><span class="sxs-lookup"><span data-stu-id="367fb-131">Valid values 0 to 255</span></span>|
|<span data-ttu-id="367fb-132">Локалпортранжес</span><span class="sxs-lookup"><span data-stu-id="367fb-132">localPortRanges</span></span>|<span data-ttu-id="367fb-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="367fb-133">String collection</span></span>|<span data-ttu-id="367fb-134">Список диапазонов локальных портов.</span><span class="sxs-lookup"><span data-stu-id="367fb-134">List of local port ranges.</span></span> <span data-ttu-id="367fb-135">Например, "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="367fb-135">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="367fb-136">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="367fb-136">If not specified, the default is All.</span></span>|
|<span data-ttu-id="367fb-137">Ремотепортранжес</span><span class="sxs-lookup"><span data-stu-id="367fb-137">remotePortRanges</span></span>|<span data-ttu-id="367fb-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="367fb-138">String collection</span></span>|<span data-ttu-id="367fb-139">Список диапазонов удаленных портов.</span><span class="sxs-lookup"><span data-stu-id="367fb-139">List of remote port ranges.</span></span> <span data-ttu-id="367fb-140">Например, "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="367fb-140">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="367fb-141">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="367fb-141">If not specified, the default is All.</span></span>|
|<span data-ttu-id="367fb-142">Локаладдрессранжес</span><span class="sxs-lookup"><span data-stu-id="367fb-142">localAddressRanges</span></span>|<span data-ttu-id="367fb-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="367fb-143">String collection</span></span>|<span data-ttu-id="367fb-144">Список локальных адресов, охваченных правилом.</span><span class="sxs-lookup"><span data-stu-id="367fb-144">List of local addresses covered by the rule.</span></span> <span data-ttu-id="367fb-145">Допустимыми являются следующие маркеры:</span><span class="sxs-lookup"><span data-stu-id="367fb-145">Valid tokens include:</span></span>
- <span data-ttu-id="367fb-146">"\*" обозначает любой локальный адрес.</span><span class="sxs-lookup"><span data-stu-id="367fb-146">"\*" indicates any local address.</span></span> <span data-ttu-id="367fb-147">Если этот параметр задан, он должен быть единственным включенным маркером.</span><span class="sxs-lookup"><span data-stu-id="367fb-147">If present, this must be the only token included.</span></span>
- <span data-ttu-id="367fb-148">Подсеть можно указать либо с помощью маски подсети, либо с помощью нотации префикса сети.</span><span class="sxs-lookup"><span data-stu-id="367fb-148">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="367fb-149">Если не указана ни маска подсети, ни префикс сети, маска подсети устанавливается по умолчанию 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="367fb-149">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="367fb-150">Допустимый IPv6-адрес.</span><span class="sxs-lookup"><span data-stu-id="367fb-150">A valid IPv6 address.</span></span>
- <span data-ttu-id="367fb-151">Диапазон IPv4-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="367fb-151">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="367fb-152">Диапазон IPv6-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="367fb-152">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="367fb-153">Значение по умолчанию — любой адрес. | | Ремотеаддрессранжес | Коллекция String | Список маркеров, указывающих удаленные адреса, покрытые правилом.</span><span class="sxs-lookup"><span data-stu-id="367fb-153">Default is any address.| |remoteAddressRanges|String collection|List of tokens specifying the remote addresses covered by the rule.</span></span> <span data-ttu-id="367fb-154">Маркеры не зависят от регистра символов.</span><span class="sxs-lookup"><span data-stu-id="367fb-154">Tokens are case insensitive.</span></span> <span data-ttu-id="367fb-155">Допустимыми являются следующие маркеры:</span><span class="sxs-lookup"><span data-stu-id="367fb-155">Valid tokens include:</span></span>
- <span data-ttu-id="367fb-156">"\*" обозначает любой удаленный адрес.</span><span class="sxs-lookup"><span data-stu-id="367fb-156">"\*" indicates any remote address.</span></span> <span data-ttu-id="367fb-157">Если этот параметр задан, он должен быть единственным включенным маркером.</span><span class="sxs-lookup"><span data-stu-id="367fb-157">If present, this must be the only token included.</span></span>
- <span data-ttu-id="367fb-158">"Дефаултгатевай"</span><span class="sxs-lookup"><span data-stu-id="367fb-158">"Defaultgateway"</span></span>
- <span data-ttu-id="367fb-159">-</span><span class="sxs-lookup"><span data-stu-id="367fb-159">"DHCP"</span></span>
- <span data-ttu-id="367fb-160">Служба</span><span class="sxs-lookup"><span data-stu-id="367fb-160">"DNS"</span></span>
- <span data-ttu-id="367fb-161">WINS</span><span class="sxs-lookup"><span data-stu-id="367fb-161">"WINS"</span></span>
- <span data-ttu-id="367fb-162">"Интрасеть" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="367fb-162">"Intranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="367fb-163">"Рмтинтранет" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="367fb-163">"RmtIntranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="367fb-164">"Интернет" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="367fb-164">"Internet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="367fb-165">"Ply2Renders" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="367fb-165">"Ply2Renders" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="367fb-166">"Локалсубнет" указывает на любой локальный адрес в локальной подсети.</span><span class="sxs-lookup"><span data-stu-id="367fb-166">"LocalSubnet" indicates any local address on the local subnet.</span></span>
- <span data-ttu-id="367fb-167">Подсеть можно указать либо с помощью маски подсети, либо с помощью нотации префикса сети.</span><span class="sxs-lookup"><span data-stu-id="367fb-167">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="367fb-168">Если не указана ни маска подсети, ни префикс сети, маска подсети устанавливается по умолчанию 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="367fb-168">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="367fb-169">Допустимый IPv6-адрес.</span><span class="sxs-lookup"><span data-stu-id="367fb-169">A valid IPv6 address.</span></span>
- <span data-ttu-id="367fb-170">Диапазон IPv4-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="367fb-170">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="367fb-171">Диапазон IPv6-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="367fb-171">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="367fb-172">Значение по умолчанию — любой адрес. | | Профилетипес | [виндовсфиреваллруленетворкпрофилетипес](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)| Задает профили, к которым относится правило.</span><span class="sxs-lookup"><span data-stu-id="367fb-172">Default is any address.| |profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Specifies the profiles to which the rule belongs.</span></span> <span data-ttu-id="367fb-173">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="367fb-173">If not specified, the default is All.</span></span> <span data-ttu-id="367fb-174">`notConfigured`Возможные значения: `domain`,, `private`, `public`. | | действие | [статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)| Действие, которое применяет правило.</span><span class="sxs-lookup"><span data-stu-id="367fb-174">Possible values are: `notConfigured`, `domain`, `private`, `public`.| |action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|The action the rule enforces.</span></span> <span data-ttu-id="367fb-175">Если этот параметр не указан, разрешено значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="367fb-175">If not specified, the default is Allowed.</span></span> <span data-ttu-id="367fb-176">Возможные значения: `notConfigured`, `blocked`, `allowed`. | | Траффикдиректион | [виндовсфиреваллрулетраффикдиректионтипе](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)| Направление трафика, для которого включено правило.</span><span class="sxs-lookup"><span data-stu-id="367fb-176">Possible values are: `notConfigured`, `blocked`, `allowed`.| |trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|The traffic direction that the rule is enabled for.</span></span> <span data-ttu-id="367fb-177">Если этот параметр не указан, используется значение по умолчанию out. Возможные значения: `notConfigured`, `out`, `in`. | | Интерфацетипес | [виндовсфиреваллрулеинтерфацетипес](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)| Типы интерфейсов правила.</span><span class="sxs-lookup"><span data-stu-id="367fb-177">If not specified, the default is Out. Possible values are: `notConfigured`, `out`, `in`.| |interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|The interface types of the rule.</span></span> <span data-ttu-id="367fb-178">`notConfigured`Возможные значения: `remoteAccess`,, `wireless`, `lan`. | | Локалусераусоризатионс | Строка | Указывает список авторизованных локальных пользователей для контейнера приложения.</span><span class="sxs-lookup"><span data-stu-id="367fb-178">Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.| |localUserAuthorizations|String|Specifies the list of authorized local users for the app container.</span></span> <span data-ttu-id="367fb-179">Это строка в формате языка определения дескрипторов безопасности (SDDL). |</span><span class="sxs-lookup"><span data-stu-id="367fb-179">This is a string in Security Descriptor Definition Language (SDDL) format.|</span></span>

## <a name="relationships"></a><span data-ttu-id="367fb-180">Связи</span><span class="sxs-lookup"><span data-stu-id="367fb-180">Relationships</span></span>
<span data-ttu-id="367fb-181">Нет</span><span class="sxs-lookup"><span data-stu-id="367fb-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="367fb-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="367fb-182">JSON Representation</span></span>
<span data-ttu-id="367fb-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="367fb-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "localUserAuthorizations": "String"
}
```




