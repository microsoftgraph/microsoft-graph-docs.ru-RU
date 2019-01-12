---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 915fab77e7a2c28ab9d6902f3e1cb7d2d05cb2b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958413"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="9312b-103">Тип перечисления firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="9312b-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="9312b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9312b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9312b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9312b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9312b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9312b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9312b-107">Возможные значения для firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="9312b-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="9312b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9312b-108">Members</span></span>
|<span data-ttu-id="9312b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9312b-109">Member</span></span>|<span data-ttu-id="9312b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9312b-110">Value</span></span>|<span data-ttu-id="9312b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9312b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9312b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9312b-112">deviceDefault</span></span>|<span data-ttu-id="9312b-113">0</span><span class="sxs-lookup"><span data-stu-id="9312b-113">0</span></span>|<span data-ttu-id="9312b-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="9312b-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="9312b-115">Нет</span><span class="sxs-lookup"><span data-stu-id="9312b-115">none</span></span>|<span data-ttu-id="9312b-116">1</span><span class="sxs-lookup"><span data-stu-id="9312b-116">1</span></span>|<span data-ttu-id="9312b-117">Не проверять списка отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="9312b-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="9312b-118">Попытка</span><span class="sxs-lookup"><span data-stu-id="9312b-118">attempt</span></span>|<span data-ttu-id="9312b-119">2</span><span class="sxs-lookup"><span data-stu-id="9312b-119">2</span></span>|<span data-ttu-id="9312b-120">Попытайтесь проверки списка отзыва Сертификатов и разрешить сертификат только в том случае, если сертификат подтверждается при проверке</span><span class="sxs-lookup"><span data-stu-id="9312b-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="9312b-121">Требовать</span><span class="sxs-lookup"><span data-stu-id="9312b-121">require</span></span>|<span data-ttu-id="9312b-122">3</span><span class="sxs-lookup"><span data-stu-id="9312b-122">3</span></span>|<span data-ttu-id="9312b-123">Требовать успешной проверки списка отзыва Сертификатов, перед тем как разрешить сертификата</span><span class="sxs-lookup"><span data-stu-id="9312b-123">Require a successful CRL check before allowing a certificate</span></span>|





