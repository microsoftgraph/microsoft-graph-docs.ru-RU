---
title: тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе
description: Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 285389d07f4ea6f667a0e12260fe5a5296808923
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524366"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="a650c-103">тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе</span><span class="sxs-lookup"><span data-stu-id="a650c-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="a650c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a650c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a650c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a650c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a650c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a650c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a650c-107">Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.</span><span class="sxs-lookup"><span data-stu-id="a650c-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="a650c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a650c-108">Members</span></span>
|<span data-ttu-id="a650c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a650c-109">Member</span></span>|<span data-ttu-id="a650c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a650c-110">Value</span></span>|<span data-ttu-id="a650c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a650c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a650c-112">нет</span><span class="sxs-lookup"><span data-stu-id="a650c-112">none</span></span>|<span data-ttu-id="a650c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a650c-113">0</span></span>|<span data-ttu-id="a650c-114">нет набора требований</span><span class="sxs-lookup"><span data-stu-id="a650c-114">no requirement set</span></span>|
|<span data-ttu-id="a650c-115">басиЦинтегрити</span><span class="sxs-lookup"><span data-stu-id="a650c-115">basicIntegrity</span></span>|<span data-ttu-id="a650c-116">1 </span><span class="sxs-lookup"><span data-stu-id="a650c-116">1</span></span>|<span data-ttu-id="a650c-117">требовать, чтобы устройство Android продавало базовую проверку целостности SafetyNet</span><span class="sxs-lookup"><span data-stu-id="a650c-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="a650c-118">басиЦинтегритянддевицецертификатион</span><span class="sxs-lookup"><span data-stu-id="a650c-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="a650c-119">2 </span><span class="sxs-lookup"><span data-stu-id="a650c-119">2</span></span>|<span data-ttu-id="a650c-120">требовать, чтобы устройство Android продавало базовую целостность SafetyNet и проверки сертификации устройств</span><span class="sxs-lookup"><span data-stu-id="a650c-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



