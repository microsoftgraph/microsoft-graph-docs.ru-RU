---
title: тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе
description: Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cef86d779a866174749a0916ab606f64374bfa1d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775473"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="c7f1d-103">тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе</span><span class="sxs-lookup"><span data-stu-id="c7f1d-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="c7f1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7f1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7f1d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7f1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7f1d-106">Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.</span><span class="sxs-lookup"><span data-stu-id="c7f1d-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="c7f1d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c7f1d-107">Members</span></span>
|<span data-ttu-id="c7f1d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c7f1d-108">Member</span></span>|<span data-ttu-id="c7f1d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c7f1d-109">Value</span></span>|<span data-ttu-id="c7f1d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f1d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f1d-111">нет</span><span class="sxs-lookup"><span data-stu-id="c7f1d-111">none</span></span>|<span data-ttu-id="c7f1d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c7f1d-112">0</span></span>|<span data-ttu-id="c7f1d-113">нет набора требований</span><span class="sxs-lookup"><span data-stu-id="c7f1d-113">no requirement set</span></span>|
|<span data-ttu-id="c7f1d-114">БасиЦинтегрити</span><span class="sxs-lookup"><span data-stu-id="c7f1d-114">basicIntegrity</span></span>|<span data-ttu-id="c7f1d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c7f1d-115">1</span></span>|<span data-ttu-id="c7f1d-116">требовать, чтобы устройство Android продавало базовую проверку целостности SafetyNet</span><span class="sxs-lookup"><span data-stu-id="c7f1d-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="c7f1d-117">БасиЦинтегритянддевицецертификатион</span><span class="sxs-lookup"><span data-stu-id="c7f1d-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="c7f1d-118">2</span><span class="sxs-lookup"><span data-stu-id="c7f1d-118">2</span></span>|<span data-ttu-id="c7f1d-119">требовать, чтобы устройство Android продавало базовую целостность SafetyNet и проверки сертификации устройств</span><span class="sxs-lookup"><span data-stu-id="c7f1d-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





