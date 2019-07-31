---
title: тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе
description: Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03c7496fe5e3d1fce5f73cc0f5954d8415668641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968080"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="330cf-103">тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе</span><span class="sxs-lookup"><span data-stu-id="330cf-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="330cf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="330cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="330cf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="330cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="330cf-106">Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.</span><span class="sxs-lookup"><span data-stu-id="330cf-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="330cf-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="330cf-107">Members</span></span>
|<span data-ttu-id="330cf-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="330cf-108">Member</span></span>|<span data-ttu-id="330cf-109">Значение</span><span class="sxs-lookup"><span data-stu-id="330cf-109">Value</span></span>|<span data-ttu-id="330cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="330cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="330cf-111">none</span><span class="sxs-lookup"><span data-stu-id="330cf-111">none</span></span>|<span data-ttu-id="330cf-112">нуль</span><span class="sxs-lookup"><span data-stu-id="330cf-112">0</span></span>|<span data-ttu-id="330cf-113">нет набора требований</span><span class="sxs-lookup"><span data-stu-id="330cf-113">no requirement set</span></span>|
|<span data-ttu-id="330cf-114">БасиЦинтегрити</span><span class="sxs-lookup"><span data-stu-id="330cf-114">basicIntegrity</span></span>|<span data-ttu-id="330cf-115">1,1</span><span class="sxs-lookup"><span data-stu-id="330cf-115">1</span></span>|<span data-ttu-id="330cf-116">требовать, чтобы устройство Android продавало базовую проверку целостности SafetyNet</span><span class="sxs-lookup"><span data-stu-id="330cf-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="330cf-117">БасиЦинтегритянддевицецертификатион</span><span class="sxs-lookup"><span data-stu-id="330cf-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="330cf-118">2</span><span class="sxs-lookup"><span data-stu-id="330cf-118">2</span></span>|<span data-ttu-id="330cf-119">требовать, чтобы устройство Android продавало базовую целостность SafetyNet и проверки сертификации устройств</span><span class="sxs-lookup"><span data-stu-id="330cf-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





