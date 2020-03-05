---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c9a94dc19064fc01d70bfa1123d20fec414eac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526446"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="677b0-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="677b0-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="677b0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="677b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="677b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="677b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="677b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="677b0-107">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="677b0-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="677b0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="677b0-108">Members</span></span>
|<span data-ttu-id="677b0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="677b0-109">Member</span></span>|<span data-ttu-id="677b0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="677b0-110">Value</span></span>|<span data-ttu-id="677b0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="677b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="677b0-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="677b0-112">deviceDefault</span></span>|<span data-ttu-id="677b0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="677b0-113">0</span></span>|<span data-ttu-id="677b0-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="677b0-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="677b0-115">нет</span><span class="sxs-lookup"><span data-stu-id="677b0-115">none</span></span>|<span data-ttu-id="677b0-116">1 </span><span class="sxs-lookup"><span data-stu-id="677b0-116">1</span></span>|<span data-ttu-id="677b0-117">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="677b0-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="677b0-118">произошл</span><span class="sxs-lookup"><span data-stu-id="677b0-118">attempt</span></span>|<span data-ttu-id="677b0-119">2 </span><span class="sxs-lookup"><span data-stu-id="677b0-119">2</span></span>|<span data-ttu-id="677b0-120">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="677b0-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="677b0-121">необходимость</span><span class="sxs-lookup"><span data-stu-id="677b0-121">require</span></span>|<span data-ttu-id="677b0-122">3 </span><span class="sxs-lookup"><span data-stu-id="677b0-122">3</span></span>|<span data-ttu-id="677b0-123">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="677b0-123">Require a successful CRL check before allowing a certificate</span></span>|



