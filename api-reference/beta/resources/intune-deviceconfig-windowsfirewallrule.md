---
title: Тип ресурса Виндовсфиреваллруле
description: Правило, контролирующее трафик через брандмауэр Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3753eeade1dce32e4332becd7575710a2f6ea1a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631611"
---
# <a name="windowsfirewallrule-resource-type"></a><span data-ttu-id="d629e-103">Тип ресурса Виндовсфиреваллруле</span><span class="sxs-lookup"><span data-stu-id="d629e-103">windowsFirewallRule resource type</span></span>

> <span data-ttu-id="d629e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d629e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d629e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d629e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d629e-106">Правило, контролирующее трафик через брандмауэр Windows.</span><span class="sxs-lookup"><span data-stu-id="d629e-106">A rule controlling traffic through the Windows Firewall.</span></span>

## <a name="properties"></a><span data-ttu-id="d629e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d629e-107">Properties</span></span>
|<span data-ttu-id="d629e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d629e-108">Property</span></span>|<span data-ttu-id="d629e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d629e-109">Type</span></span>|<span data-ttu-id="d629e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d629e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d629e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d629e-111">displayName</span></span>|<span data-ttu-id="d629e-112">String</span><span class="sxs-lookup"><span data-stu-id="d629e-112">String</span></span>|<span data-ttu-id="d629e-113">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="d629e-113">The display name of the rule.</span></span> <span data-ttu-id="d629e-114">Не обязательно должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="d629e-114">Does not need to be unique.</span></span>|
|<span data-ttu-id="d629e-115">description</span><span class="sxs-lookup"><span data-stu-id="d629e-115">description</span></span>|<span data-ttu-id="d629e-116">String</span><span class="sxs-lookup"><span data-stu-id="d629e-116">String</span></span>|<span data-ttu-id="d629e-117">Описание правила.</span><span class="sxs-lookup"><span data-stu-id="d629e-117">The description of the rule.</span></span>|
|<span data-ttu-id="d629e-118">Паккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="d629e-118">packageFamilyName</span></span>|<span data-ttu-id="d629e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="d629e-119">String</span></span>|<span data-ttu-id="d629e-120">Имя семейства пакетов приложения Microsoft Store, на которое влияет правило брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="d629e-120">The package family name of a Microsoft Store application that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="d629e-121">Пути</span><span class="sxs-lookup"><span data-stu-id="d629e-121">filePath</span></span>|<span data-ttu-id="d629e-122">Строка</span><span class="sxs-lookup"><span data-stu-id="d629e-122">String</span></span>|<span data-ttu-id="d629e-123">Полный путь к файлу приложения, на который влияет правило брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="d629e-123">The full file path of an app that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="d629e-124">Служба</span><span class="sxs-lookup"><span data-stu-id="d629e-124">serviceName</span></span>|<span data-ttu-id="d629e-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d629e-125">String</span></span>|<span data-ttu-id="d629e-126">Имя, используемое в случаях, когда служба, а не приложение, отправляет или получает трафик.</span><span class="sxs-lookup"><span data-stu-id="d629e-126">The name used in cases when a service, not an application, is sending or receiving traffic.</span></span>|
|<span data-ttu-id="d629e-127">Protocol</span><span class="sxs-lookup"><span data-stu-id="d629e-127">protocol</span></span>|<span data-ttu-id="d629e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d629e-128">Int32</span></span>|<span data-ttu-id="d629e-129">0-255 число, представляющее протокол IP (TCP = 6, UDP = 17).</span><span class="sxs-lookup"><span data-stu-id="d629e-129">0-255 number representing the IP protocol (TCP = 6, UDP = 17).</span></span> <span data-ttu-id="d629e-130">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="d629e-130">If not specified, the default is All.</span></span> <span data-ttu-id="d629e-131">Допустимые значения — от 0 до 255</span><span class="sxs-lookup"><span data-stu-id="d629e-131">Valid values 0 to 255</span></span>|
|<span data-ttu-id="d629e-132">Локалпортранжес</span><span class="sxs-lookup"><span data-stu-id="d629e-132">localPortRanges</span></span>|<span data-ttu-id="d629e-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d629e-133">String collection</span></span>|<span data-ttu-id="d629e-134">Список диапазонов локальных портов.</span><span class="sxs-lookup"><span data-stu-id="d629e-134">List of local port ranges.</span></span> <span data-ttu-id="d629e-135">Например, "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="d629e-135">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="d629e-136">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="d629e-136">If not specified, the default is All.</span></span>|
|<span data-ttu-id="d629e-137">Ремотепортранжес</span><span class="sxs-lookup"><span data-stu-id="d629e-137">remotePortRanges</span></span>|<span data-ttu-id="d629e-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d629e-138">String collection</span></span>|<span data-ttu-id="d629e-139">Список диапазонов удаленных портов.</span><span class="sxs-lookup"><span data-stu-id="d629e-139">List of remote port ranges.</span></span> <span data-ttu-id="d629e-140">Например, "100-120", "200", "300-320".</span><span class="sxs-lookup"><span data-stu-id="d629e-140">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="d629e-141">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="d629e-141">If not specified, the default is All.</span></span>|
|<span data-ttu-id="d629e-142">Локаладдрессранжес</span><span class="sxs-lookup"><span data-stu-id="d629e-142">localAddressRanges</span></span>|<span data-ttu-id="d629e-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d629e-143">String collection</span></span>|<span data-ttu-id="d629e-144">Список локальных адресов, охваченных правилом.</span><span class="sxs-lookup"><span data-stu-id="d629e-144">List of local addresses covered by the rule.</span></span> <span data-ttu-id="d629e-145">Допустимыми являются следующие маркеры:</span><span class="sxs-lookup"><span data-stu-id="d629e-145">Valid tokens include:</span></span>
- <span data-ttu-id="d629e-146">"\*" обозначает любой локальный адрес.</span><span class="sxs-lookup"><span data-stu-id="d629e-146">"\*" indicates any local address.</span></span> <span data-ttu-id="d629e-147">Если этот параметр задан, он должен быть единственным включенным маркером.</span><span class="sxs-lookup"><span data-stu-id="d629e-147">If present, this must be the only token included.</span></span>
- <span data-ttu-id="d629e-148">Подсеть можно указать либо с помощью маски подсети, либо с помощью нотации префикса сети.</span><span class="sxs-lookup"><span data-stu-id="d629e-148">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="d629e-149">Если не указана ни маска подсети, ни префикс сети, маска подсети устанавливается по умолчанию 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="d629e-149">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="d629e-150">Допустимый IPv6-адрес.</span><span class="sxs-lookup"><span data-stu-id="d629e-150">A valid IPv6 address.</span></span>
- <span data-ttu-id="d629e-151">Диапазон IPv4-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="d629e-151">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="d629e-152">Диапазон IPv6-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="d629e-152">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="d629e-153">Значение по умолчанию — любой адрес. | | Ремотеаддрессранжес | Коллекция String | Список маркеров, указывающих удаленные адреса, покрытые правилом.</span><span class="sxs-lookup"><span data-stu-id="d629e-153">Default is any address.| |remoteAddressRanges|String collection|List of tokens specifying the remote addresses covered by the rule.</span></span> <span data-ttu-id="d629e-154">Маркеры не зависят от регистра символов.</span><span class="sxs-lookup"><span data-stu-id="d629e-154">Tokens are case insensitive.</span></span> <span data-ttu-id="d629e-155">Допустимыми являются следующие маркеры:</span><span class="sxs-lookup"><span data-stu-id="d629e-155">Valid tokens include:</span></span>
- <span data-ttu-id="d629e-156">"\*" обозначает любой удаленный адрес.</span><span class="sxs-lookup"><span data-stu-id="d629e-156">"\*" indicates any remote address.</span></span> <span data-ttu-id="d629e-157">Если этот параметр задан, он должен быть единственным включенным маркером.</span><span class="sxs-lookup"><span data-stu-id="d629e-157">If present, this must be the only token included.</span></span>
- <span data-ttu-id="d629e-158">"Дефаултгатевай"</span><span class="sxs-lookup"><span data-stu-id="d629e-158">"Defaultgateway"</span></span>
- <span data-ttu-id="d629e-159">-</span><span class="sxs-lookup"><span data-stu-id="d629e-159">"DHCP"</span></span>
- <span data-ttu-id="d629e-160">Служба</span><span class="sxs-lookup"><span data-stu-id="d629e-160">"DNS"</span></span>
- <span data-ttu-id="d629e-161">WINS</span><span class="sxs-lookup"><span data-stu-id="d629e-161">"WINS"</span></span>
- <span data-ttu-id="d629e-162">"Интрасеть" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="d629e-162">"Intranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="d629e-163">"Рмтинтранет" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="d629e-163">"RmtIntranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="d629e-164">"Интернет" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="d629e-164">"Internet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="d629e-165">"Ply2Renders" (поддерживается в версиях Windows 1809 +)</span><span class="sxs-lookup"><span data-stu-id="d629e-165">"Ply2Renders" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="d629e-166">"Локалсубнет" указывает на любой локальный адрес в локальной подсети.</span><span class="sxs-lookup"><span data-stu-id="d629e-166">"LocalSubnet" indicates any local address on the local subnet.</span></span>
- <span data-ttu-id="d629e-167">Подсеть можно указать либо с помощью маски подсети, либо с помощью нотации префикса сети.</span><span class="sxs-lookup"><span data-stu-id="d629e-167">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="d629e-168">Если не указана ни маска подсети, ни префикс сети, маска подсети устанавливается по умолчанию 255.255.255.255.</span><span class="sxs-lookup"><span data-stu-id="d629e-168">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="d629e-169">Допустимый IPv6-адрес.</span><span class="sxs-lookup"><span data-stu-id="d629e-169">A valid IPv6 address.</span></span>
- <span data-ttu-id="d629e-170">Диапазон IPv4-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="d629e-170">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="d629e-171">Диапазон IPv6-адресов в формате "начальный адрес-конечный адрес" без пробелов.</span><span class="sxs-lookup"><span data-stu-id="d629e-171">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="d629e-172">Значение по умолчанию — любой адрес. | | Профилетипес | [виндовсфиреваллруленетворкпрофилетипес](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)| Задает профили, к которым относится правило.</span><span class="sxs-lookup"><span data-stu-id="d629e-172">Default is any address.| |profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Specifies the profiles to which the rule belongs.</span></span> <span data-ttu-id="d629e-173">Если этот параметр не указан, используется значение по умолчанию ALL.</span><span class="sxs-lookup"><span data-stu-id="d629e-173">If not specified, the default is All.</span></span> <span data-ttu-id="d629e-174">`notConfigured`Возможные значения: `domain`,, `private`, `public`. | | действие | [статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)| Действие, которое применяет правило.</span><span class="sxs-lookup"><span data-stu-id="d629e-174">Possible values are: `notConfigured`, `domain`, `private`, `public`.| |action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|The action the rule enforces.</span></span> <span data-ttu-id="d629e-175">Если этот параметр не указан, разрешено значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d629e-175">If not specified, the default is Allowed.</span></span> <span data-ttu-id="d629e-176">Возможные значения: `notConfigured`, `blocked`, `allowed`. | | Траффикдиректион | [виндовсфиреваллрулетраффикдиректионтипе](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)| Направление трафика, для которого включено правило.</span><span class="sxs-lookup"><span data-stu-id="d629e-176">Possible values are: `notConfigured`, `blocked`, `allowed`.| |trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|The traffic direction that the rule is enabled for.</span></span> <span data-ttu-id="d629e-177">Если этот параметр не указан, используется значение по умолчанию out. Возможные значения: `notConfigured`, `out`, `in`. | | Интерфацетипес | [виндовсфиреваллрулеинтерфацетипес](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)| Типы интерфейсов правила.</span><span class="sxs-lookup"><span data-stu-id="d629e-177">If not specified, the default is Out. Possible values are: `notConfigured`, `out`, `in`.| |interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|The interface types of the rule.</span></span> <span data-ttu-id="d629e-178">`notConfigured`Возможные значения: `remoteAccess`,, `wireless`, `lan`. | | Локалусераусоризатионс | Строка | Указывает список авторизованных локальных пользователей для контейнера приложения.</span><span class="sxs-lookup"><span data-stu-id="d629e-178">Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.| |localUserAuthorizations|String|Specifies the list of authorized local users for the app container.</span></span> <span data-ttu-id="d629e-179">Это строка в формате языка определения дескрипторов безопасности (SDDL). |</span><span class="sxs-lookup"><span data-stu-id="d629e-179">This is a string in Security Descriptor Definition Language (SDDL) format.|</span></span>

## <a name="relationships"></a><span data-ttu-id="d629e-180">Отношения</span><span class="sxs-lookup"><span data-stu-id="d629e-180">Relationships</span></span>
<span data-ttu-id="d629e-181">Нет</span><span class="sxs-lookup"><span data-stu-id="d629e-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d629e-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d629e-182">JSON Representation</span></span>
<span data-ttu-id="d629e-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d629e-183">Here is a JSON representation of the resource.</span></span>
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




