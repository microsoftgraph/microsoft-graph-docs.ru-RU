---
title: тип enum configurationManagerActionDeliveryStatus
description: Состояние доставки действия устройства Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 21de2d20718c6f1b3b0fca8199f7b6a59dcb648c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794737"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>тип enum configurationManagerActionDeliveryStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние доставки действия устройства Configuration Manager

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Ожидание доставки действия в ConfigurationManager|
|pendingDelivery|1|Ожидание доставки действия в ConfigurationManager|
|deliveredToConnectorService|2|Действие отправляется в службу Connector ConfigurationManager (облако)|
|failedToDeliverToConnectorService|3|Не удалось отправить действие в службу Connector ConfigurationManager (облако)|
|deliveredToOnPremisesServer|4 |Действие доставляется на сервер ConfigurationManager на предварительном сервере|



