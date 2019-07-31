---
title: тип перечисления Конфигуратионманажерклиентстате
description: Состояние клиента Configuration Manager
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97fd1dddcfea444d330d3f620244f8f84ebc3da0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000027"
---
# <a name="configurationmanagerclientstate-enum-type"></a>тип перечисления Конфигуратионманажерклиентстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние клиента Configuration Manager

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Агент диспетчера конфигурации старше 1806 или не установлен, или это устройство не проверялось в Intune более 30 дней.|
|устанавлива|1,1|Агент Configuration Manager установлен, но он еще не отображается в консоли Configuration Manager. Подождите несколько часов, пока оно не будет обновлено.|
|рабочее|7 |Этому устройству удалось успешно вернуть службу Configuration Manager.|
|Инсталлфаилед|8 |Не удалось установить агент диспетчера конфигураций.|
|Упдатефаилед|-11:00|Ошибка обновления от версии x до версии y агента Configuration Manager. |
|Коммуникатионеррор|19|Агенту диспетчера конфигураций удалось подключиться к службе Configuration Manager ранее, но теперь она больше не может. |





