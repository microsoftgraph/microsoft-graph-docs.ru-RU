---
title: тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе
description: Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39726acbd8daf5f8f7432b0aa633e9d992a65bba
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991928"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="bec38-103">тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе</span><span class="sxs-lookup"><span data-stu-id="bec38-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="bec38-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bec38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bec38-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bec38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bec38-106">Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.</span><span class="sxs-lookup"><span data-stu-id="bec38-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="bec38-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bec38-107">Members</span></span>
|<span data-ttu-id="bec38-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bec38-108">Member</span></span>|<span data-ttu-id="bec38-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bec38-109">Value</span></span>|<span data-ttu-id="bec38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bec38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bec38-111">none</span><span class="sxs-lookup"><span data-stu-id="bec38-111">none</span></span>|<span data-ttu-id="bec38-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bec38-112">0</span></span>|<span data-ttu-id="bec38-113">нет набора требований</span><span class="sxs-lookup"><span data-stu-id="bec38-113">no requirement set</span></span>|
|<span data-ttu-id="bec38-114">БасиЦинтегрити</span><span class="sxs-lookup"><span data-stu-id="bec38-114">basicIntegrity</span></span>|<span data-ttu-id="bec38-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bec38-115">1</span></span>|<span data-ttu-id="bec38-116">требовать, чтобы устройство Android продавало базовую проверку целостности SafetyNet</span><span class="sxs-lookup"><span data-stu-id="bec38-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="bec38-117">БасиЦинтегритянддевицецертификатион</span><span class="sxs-lookup"><span data-stu-id="bec38-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="bec38-118">2</span><span class="sxs-lookup"><span data-stu-id="bec38-118">2</span></span>|<span data-ttu-id="bec38-119">требовать, чтобы устройство Android продавало базовую целостность SafetyNet и проверки сертификации устройств</span><span class="sxs-lookup"><span data-stu-id="bec38-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





