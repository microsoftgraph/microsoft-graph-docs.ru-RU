---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92d0f13416e543e018a5a69d28751d9ddd4512c8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946639"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="b9a16-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="b9a16-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="b9a16-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9a16-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9a16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a16-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="b9a16-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="b9a16-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b9a16-107">Members</span></span>
|<span data-ttu-id="b9a16-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b9a16-108">Member</span></span>|<span data-ttu-id="b9a16-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b9a16-109">Value</span></span>|<span data-ttu-id="b9a16-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a16-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="b9a16-111">deviceDefault</span></span>|<span data-ttu-id="b9a16-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b9a16-112">0</span></span>|<span data-ttu-id="b9a16-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="b9a16-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b9a16-114">none</span><span class="sxs-lookup"><span data-stu-id="b9a16-114">none</span></span>|<span data-ttu-id="b9a16-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b9a16-115">1</span></span>|<span data-ttu-id="b9a16-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="b9a16-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="b9a16-117">произошл</span><span class="sxs-lookup"><span data-stu-id="b9a16-117">attempt</span></span>|<span data-ttu-id="b9a16-118">2</span><span class="sxs-lookup"><span data-stu-id="b9a16-118">2</span></span>|<span data-ttu-id="b9a16-119">Проверка списка ОТЗЫВА сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="b9a16-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="b9a16-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="b9a16-120">require</span></span>|<span data-ttu-id="b9a16-121">4</span><span class="sxs-lookup"><span data-stu-id="b9a16-121">3</span></span>|<span data-ttu-id="b9a16-122">Требовать успешную проверку списка ОТЗЫВА сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="b9a16-122">Require a successful CRL check before allowing a certificate</span></span>|




