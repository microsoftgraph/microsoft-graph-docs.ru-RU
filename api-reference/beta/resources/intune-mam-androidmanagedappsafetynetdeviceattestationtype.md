---
title: тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе
description: Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0ef06b8f3cc3a2e53a053f0169e5921bc02fb822
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374356"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="6c549-103">тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе</span><span class="sxs-lookup"><span data-stu-id="6c549-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="6c549-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c549-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c549-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c549-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c549-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c549-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c549-107">Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.</span><span class="sxs-lookup"><span data-stu-id="6c549-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="6c549-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6c549-108">Members</span></span>
|<span data-ttu-id="6c549-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6c549-109">Member</span></span>|<span data-ttu-id="6c549-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6c549-110">Value</span></span>|<span data-ttu-id="6c549-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6c549-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c549-112">Нет</span><span class="sxs-lookup"><span data-stu-id="6c549-112">none</span></span>|<span data-ttu-id="6c549-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6c549-113">0</span></span>|<span data-ttu-id="6c549-114">нет набора требований</span><span class="sxs-lookup"><span data-stu-id="6c549-114">no requirement set</span></span>|
|<span data-ttu-id="6c549-115">басиЦинтегрити</span><span class="sxs-lookup"><span data-stu-id="6c549-115">basicIntegrity</span></span>|<span data-ttu-id="6c549-116">1,1</span><span class="sxs-lookup"><span data-stu-id="6c549-116">1</span></span>|<span data-ttu-id="6c549-117">требовать, чтобы устройство Android продавало базовую проверку целостности SafetyNet</span><span class="sxs-lookup"><span data-stu-id="6c549-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="6c549-118">басиЦинтегритянддевицецертификатион</span><span class="sxs-lookup"><span data-stu-id="6c549-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="6c549-119">2</span><span class="sxs-lookup"><span data-stu-id="6c549-119">2</span></span>|<span data-ttu-id="6c549-120">требовать, чтобы устройство Android продавало базовую целостность SafetyNet и проверки сертификации устройств</span><span class="sxs-lookup"><span data-stu-id="6c549-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



