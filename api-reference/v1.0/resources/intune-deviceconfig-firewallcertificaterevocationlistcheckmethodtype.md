---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1eeda2493b91e63d54a45c89ed0f840288f97f43
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532528"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="9d63f-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="9d63f-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="9d63f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d63f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d63f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d63f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d63f-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="9d63f-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="9d63f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9d63f-107">Members</span></span>
|<span data-ttu-id="9d63f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9d63f-108">Member</span></span>|<span data-ttu-id="9d63f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9d63f-109">Value</span></span>|<span data-ttu-id="9d63f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d63f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d63f-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="9d63f-111">deviceDefault</span></span>|<span data-ttu-id="9d63f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9d63f-112">0</span></span>|<span data-ttu-id="9d63f-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="9d63f-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="9d63f-114">нет</span><span class="sxs-lookup"><span data-stu-id="9d63f-114">none</span></span>|<span data-ttu-id="9d63f-115">1 </span><span class="sxs-lookup"><span data-stu-id="9d63f-115">1</span></span>|<span data-ttu-id="9d63f-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="9d63f-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="9d63f-117">произошл</span><span class="sxs-lookup"><span data-stu-id="9d63f-117">attempt</span></span>|<span data-ttu-id="9d63f-118">2 </span><span class="sxs-lookup"><span data-stu-id="9d63f-118">2</span></span>|<span data-ttu-id="9d63f-119">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="9d63f-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="9d63f-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="9d63f-120">require</span></span>|<span data-ttu-id="9d63f-121">3 </span><span class="sxs-lookup"><span data-stu-id="9d63f-121">3</span></span>|<span data-ttu-id="9d63f-122">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="9d63f-122">Require a successful CRL check before allowing a certificate</span></span>|




