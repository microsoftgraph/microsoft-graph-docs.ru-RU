---
title: Управление затратами на телекоммуникации в Microsoft Intune
description: Используя Saaswedo (службу управления затратами на телекоммуникации), которая интегрируется с Intune, вы можете ограничить использование данных и роуминг на корпоративных устройствах. Эта служба позволяет настроить и применить ограничения на использование, а также отправлять пользователям оповещения при превышении настроенного порогового значения. Кроме того, вы можете настроить эту службу на выполнение различных действий, таких как отключение роуминга при превышении порогового значения. Отчеты об использовании данных и сведения о мониторинге доступны в консоли Saaswedo. Прежде чем использовать службу управления затратами на телекоммуникации Saaswedo с Intune, необходимо настроить параметры в консоли Saaswedo и в Intune. Нужно включить соединение как для службы Saaswedo, так и для Intune. Если соединение активировано только со стороны службы Saaswedo, Intune примет соединение, но проигнорирует его.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 7a23f44192b17ae2dfa745496dfbc2b4b1f5a836
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072951"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="9b4b8-109">Управление затратами на телекоммуникации в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9b4b8-109">Telecom expense management in Microsoft Intune</span></span>

<span data-ttu-id="9b4b8-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b4b8-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b4b8-111">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-111">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="9b4b8-112">Используя Saaswedo (службу управления затратами на телекоммуникации), которая интегрируется с Intune, вы можете ограничить использование данных и роуминг на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-112">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="9b4b8-113">Эта служба позволяет настроить и применить ограничения на использование, а также отправлять пользователям оповещения при превышении настроенного порогового значения.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-113">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="9b4b8-114">Кроме того, вы можете настроить эту службу на выполнение различных действий, таких как отключение роуминга при превышении порогового значения.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-114">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="9b4b8-115">Отчеты об использовании данных и сведения о мониторинге доступны в консоли Saaswedo.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-115">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="9b4b8-116">Прежде чем использовать службу управления затратами на телекоммуникации Saaswedo с Intune, необходимо настроить параметры в консоли Saaswedo и в Intune.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-116">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="9b4b8-117">Нужно включить соединение как для службы Saaswedo, так и для Intune.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-117">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="9b4b8-118">Если соединение активировано только со стороны службы Saaswedo, Intune примет соединение, но проигнорирует его.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-118">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="9b4b8-119">Для управления затратами на телекоммуникации в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="9b4b8-119">The following Graph resources are available to manage telecom expenses in Intune:</span></span>  

- [<span data-ttu-id="9b4b8-120">Партнер по управлению затратами на телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="9b4b8-120">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)






