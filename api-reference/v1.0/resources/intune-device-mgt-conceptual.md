---
title: Управление устройствами в Microsoft Intune
description: Ресурсы управления устройствами в Microsoft Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 4bd1f7dacae60fd13c1e2911e71ef7308f0b2764
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108931"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="465b8-103">Управление устройствами в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="465b8-103">Device management in Microsoft Intune</span></span>

<span data-ttu-id="465b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="465b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="465b8-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="465b8-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="465b8-106">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="465b8-106">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="465b8-107">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="465b8-107">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="465b8-108">Субъект аудита</span><span class="sxs-lookup"><span data-stu-id="465b8-108">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="465b8-109">Событие аудита</span><span class="sxs-lookup"><span data-stu-id="465b8-109">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="465b8-110">Свойство аудита</span><span class="sxs-lookup"><span data-stu-id="465b8-110">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="465b8-111">Ресурс аудита</span><span class="sxs-lookup"><span data-stu-id="465b8-111">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="465b8-112">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="465b8-112">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="465b8-113">Функции с поддержкой клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="465b8-113">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="465b8-114">Удаление пользователя из результата действия над общим устройством Apple</span><span class="sxs-lookup"><span data-stu-id="465b8-114">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="465b8-115">Обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="465b8-115">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="465b8-116">Результат действия над устройством</span><span class="sxs-lookup"><span data-stu-id="465b8-116">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="465b8-117">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="465b8-117">Device category</span></span>](intune-devices-devicecategory.md)
- [<span data-ttu-id="465b8-118">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="465b8-118">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="465b8-119">Сводка по состоянию доступа к Exchange для устройств</span><span class="sxs-lookup"><span data-stu-id="465b8-119">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="465b8-120">Геолокация устройств</span><span class="sxs-lookup"><span data-stu-id="465b8-120">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="465b8-121">Состояние подтверждения работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="465b8-121">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="465b8-122">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="465b8-122">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="465b8-123">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="465b8-123">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="465b8-124">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="465b8-124">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="465b8-125">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="465b8-125">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="465b8-126">Состояние доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="465b8-126">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="465b8-127">Причина состояния доступа к Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="465b8-127">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="465b8-128">Состояние подписки на управление устройствами</span><span class="sxs-lookup"><span data-stu-id="465b8-128">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="465b8-129">Сводка по операционной системе устройства</span><span class="sxs-lookup"><span data-stu-id="465b8-129">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="465b8-130">Состояние регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="465b8-130">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="465b8-131">Локализованное сообщение уведомления</span><span class="sxs-lookup"><span data-stu-id="465b8-131">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="465b8-132">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="465b8-132">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="465b8-133">Управляемое устройство</span><span class="sxs-lookup"><span data-stu-id="465b8-133">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="465b8-134">Обзор управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="465b8-134">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="465b8-135">Тип владельца управляемого устройства</span><span class="sxs-lookup"><span data-stu-id="465b8-135">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="465b8-136">Указанное состояние работоспособности партнера по управляемым устройствам</span><span class="sxs-lookup"><span data-stu-id="465b8-136">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="465b8-137">Тип агента управления</span><span class="sxs-lookup"><span data-stu-id="465b8-137">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="465b8-138">Шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="465b8-138">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="465b8-139">Параметры фирменной символики для шаблона уведомления</span><span class="sxs-lookup"><span data-stu-id="465b8-139">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="465b8-140">Тип платформы</span><span class="sxs-lookup"><span data-stu-id="465b8-140">Platform type</span></span>](intune-esim-platformtype.md)
- [<span data-ttu-id="465b8-141">Состояние подключения удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="465b8-141">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="465b8-142">Партнерская служба удаленного помощника</span><span class="sxs-lookup"><span data-stu-id="465b8-142">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="465b8-143">Результат действия "Удаленная блокировка"</span><span class="sxs-lookup"><span data-stu-id="465b8-143">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="465b8-144">Результат действия "Сброс секретного кода"</span><span class="sxs-lookup"><span data-stu-id="465b8-144">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="465b8-145">Tuple_2 выполнения type_ i collection_1 операции</span><span class="sxs-lookup"><span data-stu-id="465b8-145">Tuple_2 of execution type_ i collection_1 of operation</span></span>](intune-esim-tuple_2ofexecutiontype_icollection_1ofoperation.md)
- [<span data-ttu-id="465b8-146">Параметр действия "Обновление учетной записи устройства с Windows"</span><span class="sxs-lookup"><span data-stu-id="465b8-146">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="465b8-147">Пользователь</span><span class="sxs-lookup"><span data-stu-id="465b8-147">User</span></span>](intune-devices-user.md)
- [<span data-ttu-id="465b8-148">Результат действия "Проверка с помощью Защитника Windows"</span><span class="sxs-lookup"><span data-stu-id="465b8-148">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="465b8-149">Учетная запись устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="465b8-149">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="465b8-150">Учетная запись AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="465b8-150">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="465b8-151">Учетная запись Azure AD для устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="465b8-151">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)