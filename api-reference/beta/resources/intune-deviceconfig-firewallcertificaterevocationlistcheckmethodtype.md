---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ef4a78a7e61f18b52b322b4053ebfbfa7e54e05
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791760"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="0b24e-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="0b24e-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="0b24e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b24e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b24e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b24e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b24e-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="0b24e-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="0b24e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0b24e-107">Members</span></span>
|<span data-ttu-id="0b24e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0b24e-108">Member</span></span>|<span data-ttu-id="0b24e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0b24e-109">Value</span></span>|<span data-ttu-id="0b24e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0b24e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b24e-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="0b24e-111">deviceDefault</span></span>|<span data-ttu-id="0b24e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0b24e-112">0</span></span>|<span data-ttu-id="0b24e-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="0b24e-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="0b24e-114">none</span><span class="sxs-lookup"><span data-stu-id="0b24e-114">none</span></span>|<span data-ttu-id="0b24e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="0b24e-115">1</span></span>|<span data-ttu-id="0b24e-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="0b24e-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="0b24e-117">произошл</span><span class="sxs-lookup"><span data-stu-id="0b24e-117">attempt</span></span>|<span data-ttu-id="0b24e-118">2</span><span class="sxs-lookup"><span data-stu-id="0b24e-118">2</span></span>|<span data-ttu-id="0b24e-119">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="0b24e-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="0b24e-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="0b24e-120">require</span></span>|<span data-ttu-id="0b24e-121">4</span><span class="sxs-lookup"><span data-stu-id="0b24e-121">3</span></span>|<span data-ttu-id="0b24e-122">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="0b24e-122">Require a successful CRL check before allowing a certificate</span></span>|



