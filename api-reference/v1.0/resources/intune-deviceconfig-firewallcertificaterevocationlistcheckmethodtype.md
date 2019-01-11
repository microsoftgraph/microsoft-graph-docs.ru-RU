---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2beee8f7c4f049aa1918b7e1516c3ce586a8cad0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839951"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="f552b-103">Тип перечисления firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f552b-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="f552b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f552b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f552b-105">Возможные значения для firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f552b-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="f552b-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="f552b-106">Members</span></span>
|<span data-ttu-id="f552b-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="f552b-107">Member</span></span>|<span data-ttu-id="f552b-108">Значение</span><span class="sxs-lookup"><span data-stu-id="f552b-108">Value</span></span>|<span data-ttu-id="f552b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f552b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f552b-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f552b-110">deviceDefault</span></span>|<span data-ttu-id="f552b-111">0</span><span class="sxs-lookup"><span data-stu-id="f552b-111">0</span></span>|<span data-ttu-id="f552b-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="f552b-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f552b-113">Нет</span><span class="sxs-lookup"><span data-stu-id="f552b-113">none</span></span>|<span data-ttu-id="f552b-114">1</span><span class="sxs-lookup"><span data-stu-id="f552b-114">1</span></span>|<span data-ttu-id="f552b-115">Не проверять списка отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="f552b-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="f552b-116">Попытка</span><span class="sxs-lookup"><span data-stu-id="f552b-116">attempt</span></span>|<span data-ttu-id="f552b-117">2</span><span class="sxs-lookup"><span data-stu-id="f552b-117">2</span></span>|<span data-ttu-id="f552b-118">Попытайтесь проверки списка отзыва Сертификатов и разрешить сертификат только в том случае, если сертификат подтверждается при проверке</span><span class="sxs-lookup"><span data-stu-id="f552b-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="f552b-119">Требовать</span><span class="sxs-lookup"><span data-stu-id="f552b-119">require</span></span>|<span data-ttu-id="f552b-120">3</span><span class="sxs-lookup"><span data-stu-id="f552b-120">3</span></span>|<span data-ttu-id="f552b-121">Требовать успешной проверки списка отзыва Сертификатов, перед тем как разрешить сертификата</span><span class="sxs-lookup"><span data-stu-id="f552b-121">Require a successful CRL check before allowing a certificate</span></span>|



