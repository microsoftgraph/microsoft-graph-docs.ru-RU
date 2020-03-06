---
title: Управление устройствами в Microsoft Intune
description: Ресурсы по управлению устройствами в Microsoft Intune
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 435b10f59848a40e9801700ae240ad33ce0465a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530980"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="e3f64-103">Управление устройствами в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e3f64-103">Device management in Microsoft Intune</span></span>

<span data-ttu-id="e3f64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3f64-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3f64-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="e3f64-106">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="e3f64-106">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="e3f64-107">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="e3f64-107">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="e3f64-108">Субъект аудита</span><span class="sxs-lookup"><span data-stu-id="e3f64-108">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="e3f64-109">Событие аудита</span><span class="sxs-lookup"><span data-stu-id="e3f64-109">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="e3f64-110">Свойство аудита</span><span class="sxs-lookup"><span data-stu-id="e3f64-110">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="e3f64-111">Ресурс аудита</span><span class="sxs-lookup"><span data-stu-id="e3f64-111">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="e3f64-112">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="e3f64-112">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="e3f64-113">Функции с поддержкой клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="e3f64-113">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="e3f64-114">Удаление пользователя из результата действия над общим устройством Apple</span><span class="sxs-lookup"><span data-stu-id="e3f64-114">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="e3f64-115">Обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="e3f64-115">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="e3f64-116">Результат действия над устройством</span><span class="sxs-lookup"><span data-stu-id="e3f64-116">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="e3f64-117">Причина сбоя регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="e3f64-117">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="e3f64-118">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="e3f64-118">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="e3f64-119">Геолокация устройств</span><span class="sxs-lookup"><span data-stu-id="e3f64-119">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="e3f64-120">Состояние подтверждения работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="e3f64-120">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="e3f64-121">Состояние доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="e3f64-121">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="e3f64-122">Причина состояния доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="e3f64-122">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="e3f64-123">Состояние подписки на управление устройствами</span><span class="sxs-lookup"><span data-stu-id="e3f64-123">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="e3f64-124">Событие устранения проблем с управлением устройствами</span><span class="sxs-lookup"><span data-stu-id="e3f64-124">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="e3f64-125">Сводка по операционной системе устройства</span><span class="sxs-lookup"><span data-stu-id="e3f64-125">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="e3f64-126">Состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="e3f64-126">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="e3f64-127">Событие устранения проблем с регистрацией</span><span class="sxs-lookup"><span data-stu-id="e3f64-127">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="e3f64-128">Локализованное сообщение уведомления</span><span class="sxs-lookup"><span data-stu-id="e3f64-128">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="e3f64-129">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="e3f64-129">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="e3f64-130">Управляемое устройство</span><span class="sxs-lookup"><span data-stu-id="e3f64-130">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="e3f64-131">Обзор управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="e3f64-131">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="e3f64-132">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="e3f64-132">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="e3f64-133">Указанное состояние работоспособности партнера по управляемым устройствам</span><span class="sxs-lookup"><span data-stu-id="e3f64-133">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="e3f64-134">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="e3f64-134">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="e3f64-135">Шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="e3f64-135">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="e3f64-136">Параметры фирменной символики для шаблона уведомления</span><span class="sxs-lookup"><span data-stu-id="e3f64-136">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="e3f64-137">Состояние подключения удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="e3f64-137">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="e3f64-138">Партнерская служба удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="e3f64-138">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="e3f64-139">Результат действия "Удаленная блокировка"</span><span class="sxs-lookup"><span data-stu-id="e3f64-139">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="e3f64-140">Результат действия "Сброс секретного кода"</span><span class="sxs-lookup"><span data-stu-id="e3f64-140">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="e3f64-141">Параметр действия "Обновление учетной записи устройства с Windows"</span><span class="sxs-lookup"><span data-stu-id="e3f64-141">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="e3f64-142">Результат действия "Проверка с помощью Защитника Windows"</span><span class="sxs-lookup"><span data-stu-id="e3f64-142">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="e3f64-143">Учетная запись устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="e3f64-143">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="e3f64-144">Учетная запись AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="e3f64-144">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="e3f64-145">Учетная запись Azure AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="e3f64-145">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)

