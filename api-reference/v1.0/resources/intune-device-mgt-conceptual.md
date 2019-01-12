---
title: Управление устройствами в Microsoft Intune
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d665b70f812a18f840ce43a029fe0729d454745
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980645"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="b2a62-102">Управление устройствами в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b2a62-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="b2a62-103">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2a62-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="b2a62-104">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="b2a62-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="b2a62-105">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="b2a62-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="b2a62-106">Субъект аудита</span><span class="sxs-lookup"><span data-stu-id="b2a62-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="b2a62-107">Событие аудита</span><span class="sxs-lookup"><span data-stu-id="b2a62-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="b2a62-108">Свойство аудита</span><span class="sxs-lookup"><span data-stu-id="b2a62-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="b2a62-109">Ресурс аудита</span><span class="sxs-lookup"><span data-stu-id="b2a62-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="b2a62-110">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="b2a62-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="b2a62-111">Функции с поддержкой клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="b2a62-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="b2a62-112">Удаление пользователя из результата действия над общим устройством Apple</span><span class="sxs-lookup"><span data-stu-id="b2a62-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="b2a62-113">Обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="b2a62-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="b2a62-114">Результат действия над устройством</span><span class="sxs-lookup"><span data-stu-id="b2a62-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="b2a62-115">Причина сбоя устройства подачи заявок</span><span class="sxs-lookup"><span data-stu-id="b2a62-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="b2a62-116">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="b2a62-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="b2a62-117">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="b2a62-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="b2a62-118">Геолокация устройств</span><span class="sxs-lookup"><span data-stu-id="b2a62-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="b2a62-119">Состояние подтверждения работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="b2a62-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="b2a62-120">Состояние доступа устройства управления exchange</span><span class="sxs-lookup"><span data-stu-id="b2a62-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="b2a62-121">Устройство управления exchange доступа состояние причине</span><span class="sxs-lookup"><span data-stu-id="b2a62-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="b2a62-122">Состояния подписки управления устройства</span><span class="sxs-lookup"><span data-stu-id="b2a62-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="b2a62-123">Событие устранения проблем с управлением устройствами</span><span class="sxs-lookup"><span data-stu-id="b2a62-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="b2a62-124">Сводка по операционной системе устройства</span><span class="sxs-lookup"><span data-stu-id="b2a62-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="b2a62-125">Состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="b2a62-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="b2a62-126">Событие устранения проблем с регистрацией</span><span class="sxs-lookup"><span data-stu-id="b2a62-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="b2a62-127">Локализованное сообщение уведомления</span><span class="sxs-lookup"><span data-stu-id="b2a62-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="b2a62-128">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="b2a62-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="b2a62-129">Управляемое устройство</span><span class="sxs-lookup"><span data-stu-id="b2a62-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="b2a62-130">Обзор управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="b2a62-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="b2a62-131">Управляемый тип устройства владельцем</span><span class="sxs-lookup"><span data-stu-id="b2a62-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="b2a62-132">Управляемые устройства партнера состояние работоспособности</span><span class="sxs-lookup"><span data-stu-id="b2a62-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="b2a62-133">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="b2a62-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="b2a62-134">Шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="b2a62-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="b2a62-135">Шаблон уведомления для фирменной настройки параметров</span><span class="sxs-lookup"><span data-stu-id="b2a62-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="b2a62-136">Состояние на использование доски удаленный помощник</span><span class="sxs-lookup"><span data-stu-id="b2a62-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="b2a62-137">Партнерская служба удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="b2a62-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="b2a62-138">Результат действия "Удаленная блокировка"</span><span class="sxs-lookup"><span data-stu-id="b2a62-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="b2a62-139">Результат действия "Сброс секретного кода"</span><span class="sxs-lookup"><span data-stu-id="b2a62-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="b2a62-140">Параметр действия "Обновление учетной записи устройства с Windows"</span><span class="sxs-lookup"><span data-stu-id="b2a62-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="b2a62-141">Результат действия "Проверка с помощью Защитника Windows"</span><span class="sxs-lookup"><span data-stu-id="b2a62-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="b2a62-142">Учетная запись устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="b2a62-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="b2a62-143">Учетная запись AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="b2a62-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="b2a62-144">Учетная запись Azure AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="b2a62-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
