---
title: тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе
description: Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: eb21ce8d54b006db4e98828eb7c8240dd2810b14
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332325"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="5f437-103">тип перечисления Андроидманажедаппсафетинетдевицеаттестатионтипе</span><span class="sxs-lookup"><span data-stu-id="5f437-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="5f437-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f437-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f437-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f437-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f437-106">Для управляемого приложения требуется, чтобы администратор применяет SafetyNet аттестации устройств Android.</span><span class="sxs-lookup"><span data-stu-id="5f437-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="5f437-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5f437-107">Members</span></span>
|<span data-ttu-id="5f437-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5f437-108">Member</span></span>|<span data-ttu-id="5f437-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5f437-109">Value</span></span>|<span data-ttu-id="5f437-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f437-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f437-111">none</span><span class="sxs-lookup"><span data-stu-id="5f437-111">none</span></span>|<span data-ttu-id="5f437-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5f437-112">0</span></span>|<span data-ttu-id="5f437-113">нет набора требований</span><span class="sxs-lookup"><span data-stu-id="5f437-113">no requirement set</span></span>|
|<span data-ttu-id="5f437-114">басиЦинтегрити</span><span class="sxs-lookup"><span data-stu-id="5f437-114">basicIntegrity</span></span>|<span data-ttu-id="5f437-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5f437-115">1</span></span>|<span data-ttu-id="5f437-116">требовать, чтобы устройство Android продавало базовую проверку целостности SafetyNet</span><span class="sxs-lookup"><span data-stu-id="5f437-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="5f437-117">басиЦинтегритянддевицецертификатион</span><span class="sxs-lookup"><span data-stu-id="5f437-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="5f437-118">2</span><span class="sxs-lookup"><span data-stu-id="5f437-118">2</span></span>|<span data-ttu-id="5f437-119">требовать, чтобы устройство Android продавало базовую целостность SafetyNet и проверки сертификации устройств</span><span class="sxs-lookup"><span data-stu-id="5f437-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



