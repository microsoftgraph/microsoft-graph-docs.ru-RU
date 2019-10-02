---
title: Управление устройствами в Microsoft Intune
description: Ресурсы по управлению устройствами в Microsoft Intune
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 93af3003f76d87bb49fc7b71735ef3b7209d3baf
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360372"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="226af-103">Управление устройствами в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="226af-103">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="226af-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="226af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="226af-105">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="226af-105">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="226af-106">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="226af-106">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="226af-107">Субъект аудита</span><span class="sxs-lookup"><span data-stu-id="226af-107">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="226af-108">Событие аудита</span><span class="sxs-lookup"><span data-stu-id="226af-108">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="226af-109">Свойство аудита</span><span class="sxs-lookup"><span data-stu-id="226af-109">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="226af-110">Ресурс аудита</span><span class="sxs-lookup"><span data-stu-id="226af-110">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="226af-111">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="226af-111">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="226af-112">Функции с поддержкой клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="226af-112">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="226af-113">Удаление пользователя из результата действия над общим устройством Apple</span><span class="sxs-lookup"><span data-stu-id="226af-113">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="226af-114">Обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="226af-114">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="226af-115">Результат действия над устройством</span><span class="sxs-lookup"><span data-stu-id="226af-115">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="226af-116">Причина сбоя регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="226af-116">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="226af-117">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="226af-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="226af-118">Геолокация устройств</span><span class="sxs-lookup"><span data-stu-id="226af-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="226af-119">Состояние подтверждения работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="226af-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="226af-120">Состояние доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="226af-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="226af-121">Причина состояния доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="226af-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="226af-122">Состояние подписки на управление устройствами</span><span class="sxs-lookup"><span data-stu-id="226af-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="226af-123">Событие устранения проблем с управлением устройствами</span><span class="sxs-lookup"><span data-stu-id="226af-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="226af-124">Сводка по операционной системе устройства</span><span class="sxs-lookup"><span data-stu-id="226af-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="226af-125">Состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="226af-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="226af-126">Событие устранения проблем с регистрацией</span><span class="sxs-lookup"><span data-stu-id="226af-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="226af-127">Локализованное сообщение уведомления</span><span class="sxs-lookup"><span data-stu-id="226af-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="226af-128">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="226af-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="226af-129">Управляемое устройство</span><span class="sxs-lookup"><span data-stu-id="226af-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="226af-130">Обзор управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="226af-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="226af-131">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="226af-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="226af-132">Указанное состояние работоспособности партнера по управляемым устройствам</span><span class="sxs-lookup"><span data-stu-id="226af-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="226af-133">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="226af-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="226af-134">Шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="226af-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="226af-135">Параметры фирменной символики для шаблона уведомления</span><span class="sxs-lookup"><span data-stu-id="226af-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="226af-136">Состояние подключения удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="226af-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="226af-137">Партнерская служба удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="226af-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="226af-138">Результат действия "Удаленная блокировка"</span><span class="sxs-lookup"><span data-stu-id="226af-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="226af-139">Результат действия "Сброс секретного кода"</span><span class="sxs-lookup"><span data-stu-id="226af-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="226af-140">Параметр действия "Обновление учетной записи устройства с Windows"</span><span class="sxs-lookup"><span data-stu-id="226af-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="226af-141">Результат действия "Проверка с помощью Защитника Windows"</span><span class="sxs-lookup"><span data-stu-id="226af-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="226af-142">Учетная запись устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="226af-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="226af-143">Учетная запись AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="226af-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="226af-144">Учетная запись Azure AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="226af-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)

