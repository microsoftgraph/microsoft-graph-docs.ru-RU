---
title: 'Управление затратами на телекоммуникации в Microsoft Intune : API Microsoft Graph'
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), связанных с управлением затратами на телекоммуникации для организации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 471bd6315c35b713bb022cc9872f96ac70fcd050
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159474"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="1c7bb-103">Управление затратами на телекоммуникации в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1c7bb-103">Telecom expense management in Microsoft Intune</span></span>

<span data-ttu-id="1c7bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c7bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c7bb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c7bb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c7bb-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c7bb-108">Используя Saaswedo (службу управления затратами на телекоммуникации), которая интегрируется с Intune, вы можете ограничить использование данных и роуминг на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-108">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="1c7bb-109">Эта служба позволяет настроить и применить ограничения на использование, а также отправлять пользователям оповещения при превышении настроенного порогового значения.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-109">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="1c7bb-110">Кроме того, вы можете настроить эту службу на выполнение различных действий, таких как отключение роуминга при превышении порогового значения.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-110">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="1c7bb-111">Отчеты об использовании данных и сведения о мониторинге доступны в консоли Saaswedo.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-111">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="1c7bb-112">Прежде чем использовать службу управления затратами на телекоммуникации Saaswedo с Intune, необходимо настроить параметры в консоли Saaswedo и в Intune.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-112">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="1c7bb-113">Нужно включить соединение как для службы Saaswedo, так и для Intune.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-113">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="1c7bb-114">Если соединение активировано только со стороны службы Saaswedo, Intune примет соединение, но проигнорирует его.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-114">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="1c7bb-115">Для управления затратами на телекоммуникации в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="1c7bb-115">The following Graph resources are available to manage telecom expenses in Intune:</span></span>

- [<span data-ttu-id="1c7bb-116">Партнер по управлению затратами на телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="1c7bb-116">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)