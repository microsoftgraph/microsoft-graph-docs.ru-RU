---
title: Управление расходами на телекоммуникации в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), связанных с управлением расходами на телекоммуникации в организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 08582cfe5a041db9cd8b17bfca6fab14c7ae864a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967317"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="57e59-103">Управление затратами на телекоммуникации в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="57e59-103">Telecom expense management in Microsoft Intune</span></span>

> <span data-ttu-id="57e59-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57e59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57e59-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57e59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57e59-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57e59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57e59-107">Используя Saaswedo (службу управления затратами на телекоммуникации), которая интегрируется с Intune, вы можете ограничить использование данных и роуминг на корпоративных устройствах.</span><span class="sxs-lookup"><span data-stu-id="57e59-107">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="57e59-108">Эта служба позволяет настроить и применить ограничения на использование, а также отправлять пользователям оповещения при превышении настроенного порогового значения.</span><span class="sxs-lookup"><span data-stu-id="57e59-108">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="57e59-109">Кроме того, вы можете настроить эту службу на выполнение различных действий, таких как отключение роуминга при превышении порогового значения.</span><span class="sxs-lookup"><span data-stu-id="57e59-109">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="57e59-110">Отчеты об использовании данных и сведения о мониторинге доступны в консоли Saaswedo.</span><span class="sxs-lookup"><span data-stu-id="57e59-110">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="57e59-111">Прежде чем использовать службу управления затратами на телекоммуникации Saaswedo с Intune, необходимо настроить параметры в консоли Saaswedo и в Intune.</span><span class="sxs-lookup"><span data-stu-id="57e59-111">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="57e59-112">Нужно включить соединение как для службы Saaswedo, так и для Intune.</span><span class="sxs-lookup"><span data-stu-id="57e59-112">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="57e59-113">Если соединение активировано только со стороны службы Saaswedo, Intune примет соединение, но проигнорирует его.</span><span class="sxs-lookup"><span data-stu-id="57e59-113">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="57e59-114">Для управления затратами на телекоммуникации в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="57e59-114">The following Graph resources are available to manage telecom expenses in Intune:</span></span>

- [<span data-ttu-id="57e59-115">Партнер по управлению затратами на телекоммуникации</span><span class="sxs-lookup"><span data-stu-id="57e59-115">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)
