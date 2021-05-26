---
title: тип enum deviceManagementConfigurationTemplateFamily
description: Описывает объект TemplateFamily для объекта Template
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 088e1ccd80e59b95419c17d532c82c1ea9c388bc
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666690"
---
# <a name="devicemanagementconfigurationtemplatefamily-enum-type"></a><span data-ttu-id="b5257-103">тип enum deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="b5257-103">deviceManagementConfigurationTemplateFamily enum type</span></span>

<span data-ttu-id="b5257-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5257-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5257-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5257-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5257-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5257-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5257-107">Описывает объект TemplateFamily для объекта Template</span><span class="sxs-lookup"><span data-stu-id="b5257-107">Describes the TemplateFamily for the Template entity</span></span>

## <a name="members"></a><span data-ttu-id="b5257-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b5257-108">Members</span></span>
|<span data-ttu-id="b5257-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b5257-109">Member</span></span>|<span data-ttu-id="b5257-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b5257-110">Value</span></span>|<span data-ttu-id="b5257-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5257-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5257-112">нет</span><span class="sxs-lookup"><span data-stu-id="b5257-112">none</span></span>|<span data-ttu-id="b5257-113">0</span><span class="sxs-lookup"><span data-stu-id="b5257-113">0</span></span>|<span data-ttu-id="b5257-114">По умолчанию для семейства шаблонов, когда политика не связана с шаблоном</span><span class="sxs-lookup"><span data-stu-id="b5257-114">Default for Template Family when Policy is not linked to a Template</span></span>|
|<span data-ttu-id="b5257-115">endpointSecurityAntivirus</span><span class="sxs-lookup"><span data-stu-id="b5257-115">endpointSecurityAntivirus</span></span>|<span data-ttu-id="b5257-116">10 </span><span class="sxs-lookup"><span data-stu-id="b5257-116">10</span></span>|<span data-ttu-id="b5257-117">Семейство шаблонов для endpointSecurityAntivirus, которое управляет дискретной группой параметров антивируса для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="b5257-117">Template Family for EndpointSecurityAntivirus that manages the discrete group of antivirus settings for managed devices</span></span>|
|<span data-ttu-id="b5257-118">endpointSecurityDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="b5257-118">endpointSecurityDiskEncryption</span></span>|<span data-ttu-id="b5257-119">11</span><span class="sxs-lookup"><span data-stu-id="b5257-119">11</span></span>|<span data-ttu-id="b5257-120">Семейство шаблонов для endpointSecurityDiskEncryption, которое предоставляет параметры, которые актуальны для встроенного метода шифрования устройств, например FileVault или BitLocker</span><span class="sxs-lookup"><span data-stu-id="b5257-120">Template Family for EndpointSecurityDiskEncryption that provides settings that are relevant for a devices built-in encryption  method, like FileVault or BitLocker</span></span>|
|<span data-ttu-id="b5257-121">endpointSecurityFirewall</span><span class="sxs-lookup"><span data-stu-id="b5257-121">endpointSecurityFirewall</span></span>|<span data-ttu-id="b5257-122">12 </span><span class="sxs-lookup"><span data-stu-id="b5257-122">12</span></span>|<span data-ttu-id="b5257-123">Семейство шаблонов для EndpointSecurityFirewall, которое помогает настроить встроенный брандмауэр устройств для устройств с macOS и Windows 10</span><span class="sxs-lookup"><span data-stu-id="b5257-123">Template Family for EndpointSecurityFirewall that helps configure a devices built-in firewall for device that run macOS and Windows 10</span></span>|
|<span data-ttu-id="b5257-124">endpointSecurityEndpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="b5257-124">endpointSecurityEndpointDetectionAndResponse</span></span>|<span data-ttu-id="b5257-125">13</span><span class="sxs-lookup"><span data-stu-id="b5257-125">13</span></span>|<span data-ttu-id="b5257-126">Семейство шаблонов для EndpointSecurityEndpointDectionAndResponse, которое упрощает управление настройками EDR и бортовых устройств в Microsoft Defender для Endpoint</span><span class="sxs-lookup"><span data-stu-id="b5257-126">Template Family for EndpointSecurityEndpointDectionAndResponse that facilitates management of the EDR settings and onboard devices to Microsoft Defender for Endpoint</span></span>|
|<span data-ttu-id="b5257-127">endpointSecurityAttackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="b5257-127">endpointSecurityAttackSurfaceReduction</span></span>|<span data-ttu-id="b5257-128">14 </span><span class="sxs-lookup"><span data-stu-id="b5257-128">14</span></span>|<span data-ttu-id="b5257-129">Семейство шаблонов для EndpointSecurityAttackSurfaceReduction, которое помогает уменьшить поверхности атак, минимизируя места, в которых ваша организация уязвима для киберугроз и атак</span><span class="sxs-lookup"><span data-stu-id="b5257-129">Template Family for EndpointSecurityAttackSurfaceReduction that help reduce your attack surfaces, by minimizing the places where your organization is vulnerable to cyberthreats and attacks</span></span>|
|<span data-ttu-id="b5257-130">endpointSecurityAccountProtection</span><span class="sxs-lookup"><span data-stu-id="b5257-130">endpointSecurityAccountProtection</span></span>|<span data-ttu-id="b5257-131">15</span><span class="sxs-lookup"><span data-stu-id="b5257-131">15</span></span>|<span data-ttu-id="b5257-132">Семейство шаблонов для EndpointSecurityAccountProtection, облегчающего защиту удостоверений и учетных записей пользователей</span><span class="sxs-lookup"><span data-stu-id="b5257-132">Template Family for EndpointSecurityAccountProtection that facilitates protecting the identity and accounts of users</span></span>|
|<span data-ttu-id="b5257-133">endpointSecurityApplicationControl</span><span class="sxs-lookup"><span data-stu-id="b5257-133">endpointSecurityApplicationControl</span></span>|<span data-ttu-id="b5257-134">16 </span><span class="sxs-lookup"><span data-stu-id="b5257-134">16</span></span>|<span data-ttu-id="b5257-135">Семейство шаблонов для applicationControl, которое помогает уменьшить угрозы безопасности, ограничивая приложения, которые могут запускать пользователи, и код, который выполняется в ядре System Core (ядра)</span><span class="sxs-lookup"><span data-stu-id="b5257-135">Template Family for ApplicationControl that helps mitigate security threats by restricting the applications that users can run and the code that runs in the System Core (kernel)</span></span>|




