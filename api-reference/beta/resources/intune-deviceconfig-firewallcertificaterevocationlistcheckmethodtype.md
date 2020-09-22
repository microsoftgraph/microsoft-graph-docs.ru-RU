---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e5c3f9d338ae0a5bf047bb0e8a18d7e7fdb94593
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994129"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="d04b8-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="d04b8-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="d04b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d04b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d04b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d04b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d04b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d04b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d04b8-107">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="d04b8-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="d04b8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d04b8-108">Members</span></span>
|<span data-ttu-id="d04b8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d04b8-109">Member</span></span>|<span data-ttu-id="d04b8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d04b8-110">Value</span></span>|<span data-ttu-id="d04b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d04b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d04b8-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="d04b8-112">deviceDefault</span></span>|<span data-ttu-id="d04b8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d04b8-113">0</span></span>|<span data-ttu-id="d04b8-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="d04b8-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d04b8-115">Нет</span><span class="sxs-lookup"><span data-stu-id="d04b8-115">none</span></span>|<span data-ttu-id="d04b8-116">1 </span><span class="sxs-lookup"><span data-stu-id="d04b8-116">1</span></span>|<span data-ttu-id="d04b8-117">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="d04b8-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="d04b8-118">произошл</span><span class="sxs-lookup"><span data-stu-id="d04b8-118">attempt</span></span>|<span data-ttu-id="d04b8-119">2 </span><span class="sxs-lookup"><span data-stu-id="d04b8-119">2</span></span>|<span data-ttu-id="d04b8-120">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="d04b8-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="d04b8-121">необходимость</span><span class="sxs-lookup"><span data-stu-id="d04b8-121">require</span></span>|<span data-ttu-id="d04b8-122">4</span><span class="sxs-lookup"><span data-stu-id="d04b8-122">3</span></span>|<span data-ttu-id="d04b8-123">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="d04b8-123">Require a successful CRL check before allowing a certificate</span></span>|






