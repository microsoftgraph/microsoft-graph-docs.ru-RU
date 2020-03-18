---
title: тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе
description: Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 93d65431cfcdfc952231237f2646eee79e331ef3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782701"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="dae2e-103">тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе</span><span class="sxs-lookup"><span data-stu-id="dae2e-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="dae2e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dae2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dae2e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dae2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dae2e-106">Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.</span><span class="sxs-lookup"><span data-stu-id="dae2e-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="dae2e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="dae2e-107">Members</span></span>
|<span data-ttu-id="dae2e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="dae2e-108">Member</span></span>|<span data-ttu-id="dae2e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="dae2e-109">Value</span></span>|<span data-ttu-id="dae2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dae2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dae2e-111">none</span><span class="sxs-lookup"><span data-stu-id="dae2e-111">none</span></span>|<span data-ttu-id="dae2e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="dae2e-112">0</span></span>|<span data-ttu-id="dae2e-113">нет набора требований</span><span class="sxs-lookup"><span data-stu-id="dae2e-113">no requirement set</span></span>|
|<span data-ttu-id="dae2e-114">басиЦинтегрити</span><span class="sxs-lookup"><span data-stu-id="dae2e-114">basicIntegrity</span></span>|<span data-ttu-id="dae2e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="dae2e-115">1</span></span>|<span data-ttu-id="dae2e-116">требовать, чтобы устройство Android продавало базовую проверку целостности SafetyNet</span><span class="sxs-lookup"><span data-stu-id="dae2e-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="dae2e-117">басиЦинтегритянддевицецертификатион</span><span class="sxs-lookup"><span data-stu-id="dae2e-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="dae2e-118">2</span><span class="sxs-lookup"><span data-stu-id="dae2e-118">2</span></span>|<span data-ttu-id="dae2e-119">требовать, чтобы устройство Android продавало базовую целостность SafetyNet и проверки сертификации устройств</span><span class="sxs-lookup"><span data-stu-id="dae2e-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



