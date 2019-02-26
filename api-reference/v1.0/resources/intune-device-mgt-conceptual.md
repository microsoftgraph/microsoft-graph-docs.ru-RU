---
title: Управление устройствами в Microsoft Intune
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4c8f6676647405e8186e9d27466266f6690e2cd1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250070"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="36804-102">Управление устройствами в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="36804-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="36804-103">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36804-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="36804-104">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="36804-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="36804-105">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="36804-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="36804-106">Субъект аудита</span><span class="sxs-lookup"><span data-stu-id="36804-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="36804-107">Событие аудита</span><span class="sxs-lookup"><span data-stu-id="36804-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="36804-108">Свойство аудита</span><span class="sxs-lookup"><span data-stu-id="36804-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="36804-109">Ресурс аудита</span><span class="sxs-lookup"><span data-stu-id="36804-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="36804-110">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="36804-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="36804-111">Функции с поддержкой клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="36804-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="36804-112">Удаление пользователя из результата действия над общим устройством Apple</span><span class="sxs-lookup"><span data-stu-id="36804-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="36804-113">Обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="36804-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="36804-114">Результат действия над устройством</span><span class="sxs-lookup"><span data-stu-id="36804-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="36804-115">Причина сбоя регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="36804-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="36804-116">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="36804-116">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="36804-117">Геолокация устройств</span><span class="sxs-lookup"><span data-stu-id="36804-117">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="36804-118">Состояние подтверждения работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="36804-118">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="36804-119">Состояние доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="36804-119">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="36804-120">Причина состояния доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="36804-120">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="36804-121">Состояние подписки на управление устройствами</span><span class="sxs-lookup"><span data-stu-id="36804-121">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="36804-122">Событие устранения проблем с управлением устройствами</span><span class="sxs-lookup"><span data-stu-id="36804-122">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="36804-123">Сводка по операционной системе устройства</span><span class="sxs-lookup"><span data-stu-id="36804-123">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="36804-124">Состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="36804-124">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="36804-125">Событие устранения проблем с регистрацией</span><span class="sxs-lookup"><span data-stu-id="36804-125">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="36804-126">Локализованное сообщение уведомления</span><span class="sxs-lookup"><span data-stu-id="36804-126">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="36804-127">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="36804-127">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="36804-128">Управляемое устройство</span><span class="sxs-lookup"><span data-stu-id="36804-128">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="36804-129">Обзор управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="36804-129">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="36804-130">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="36804-130">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="36804-131">Указанное состояние работоспособности партнера по управляемым устройствам</span><span class="sxs-lookup"><span data-stu-id="36804-131">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="36804-132">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="36804-132">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="36804-133">Шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="36804-133">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="36804-134">Параметры фирменной символики для шаблона уведомления</span><span class="sxs-lookup"><span data-stu-id="36804-134">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="36804-135">Состояние подключения удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="36804-135">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="36804-136">Партнерская служба удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="36804-136">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="36804-137">Результат действия "Удаленная блокировка"</span><span class="sxs-lookup"><span data-stu-id="36804-137">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="36804-138">Результат действия "Сброс секретного кода"</span><span class="sxs-lookup"><span data-stu-id="36804-138">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="36804-139">Параметр действия "Обновление учетной записи устройства с Windows"</span><span class="sxs-lookup"><span data-stu-id="36804-139">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="36804-140">Результат действия "Проверка с помощью Защитника Windows"</span><span class="sxs-lookup"><span data-stu-id="36804-140">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="36804-141">Учетная запись устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="36804-141">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="36804-142">Учетная запись AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="36804-142">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="36804-143">Учетная запись Azure AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="36804-143">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
