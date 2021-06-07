---
title: Управление устройствами в Microsoft Intune
description: Ресурсы управления устройствами в Microsoft Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 80c643d4d1c75c27df35a85a576f93838dd03554
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732714"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="1ab74-103">Управление устройствами в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1ab74-103">Device management in Microsoft Intune</span></span>

<span data-ttu-id="1ab74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ab74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ab74-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ab74-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="1ab74-106">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="1ab74-106">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="1ab74-107">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="1ab74-107">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="1ab74-108">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="1ab74-108">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="1ab74-109">Функции с поддержкой клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="1ab74-109">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="1ab74-110">Удаление пользователя из результата действия над общим устройством Apple</span><span class="sxs-lookup"><span data-stu-id="1ab74-110">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="1ab74-111">Обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="1ab74-111">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="1ab74-112">Результат действия над устройством</span><span class="sxs-lookup"><span data-stu-id="1ab74-112">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="1ab74-113">Причина сбоя регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="1ab74-113">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="1ab74-114">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="1ab74-114">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="1ab74-115">Геолокация устройств</span><span class="sxs-lookup"><span data-stu-id="1ab74-115">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="1ab74-116">Состояние подтверждения работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="1ab74-116">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="1ab74-117">Состояние доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="1ab74-117">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="1ab74-118">Причина состояния доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="1ab74-118">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="1ab74-119">Состояние подписки на управление устройствами</span><span class="sxs-lookup"><span data-stu-id="1ab74-119">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="1ab74-120">Событие устранения проблем с управлением устройствами</span><span class="sxs-lookup"><span data-stu-id="1ab74-120">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="1ab74-121">Сводка по операционной системе устройства</span><span class="sxs-lookup"><span data-stu-id="1ab74-121">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="1ab74-122">Состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="1ab74-122">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="1ab74-123">Событие устранения проблем с регистрацией</span><span class="sxs-lookup"><span data-stu-id="1ab74-123">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="1ab74-124">Локализованное сообщение уведомления</span><span class="sxs-lookup"><span data-stu-id="1ab74-124">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="1ab74-125">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="1ab74-125">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="1ab74-126">Управляемое устройство</span><span class="sxs-lookup"><span data-stu-id="1ab74-126">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="1ab74-127">Обзор управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="1ab74-127">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="1ab74-128">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="1ab74-128">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="1ab74-129">Указанное состояние работоспособности партнера по управляемым устройствам</span><span class="sxs-lookup"><span data-stu-id="1ab74-129">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="1ab74-130">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="1ab74-130">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="1ab74-131">Шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="1ab74-131">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="1ab74-132">Параметры фирменной символики для шаблона уведомления</span><span class="sxs-lookup"><span data-stu-id="1ab74-132">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="1ab74-133">Состояние подключения удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="1ab74-133">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="1ab74-134">Партнерская служба удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="1ab74-134">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="1ab74-135">Результат действия "Удаленная блокировка"</span><span class="sxs-lookup"><span data-stu-id="1ab74-135">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="1ab74-136">Результат действия "Сброс секретного кода"</span><span class="sxs-lookup"><span data-stu-id="1ab74-136">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="1ab74-137">Параметр действия "Обновление учетной записи устройства с Windows"</span><span class="sxs-lookup"><span data-stu-id="1ab74-137">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="1ab74-138">Результат действия "Проверка с помощью Защитника Windows"</span><span class="sxs-lookup"><span data-stu-id="1ab74-138">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="1ab74-139">Учетная запись устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="1ab74-139">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="1ab74-140">Учетная запись AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="1ab74-140">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="1ab74-141">Учетная запись Azure AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="1ab74-141">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)






